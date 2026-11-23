# BLOON GSV Archaeology — Normalized Data Model

**Status:** schema design / migration target. This is not a claim that legacy CSV rows have already been migrated.

## Why normalize?

The survey has three different things that must not share one row identity:

1. **Site** — a physical place or spatial container: building, corner, plaza, industrial complex, residential frontage.
2. **POI** — a business, institution, service, or other named entity associated with a site.
3. **Observation** — one appearance/evidence event: image angle, capture date, visible sign, listing panel, or replay.

One plaza may contain many businesses. One business may appear in many images and years. A building may host several tenants. Therefore, site, POI, and observation records are separate.

## Core entities

### sites
- site_id: stable internal identifier; never derive from a batch number alone.
- site_name: optional descriptive name; use only when supported.
- site_type: STANDALONE, PLAZA, INDUSTRIAL_COMPLEX, RESIDENTIAL_FRONTAGE, INSTITUTIONAL_SITE, MIXED_USE, UNKNOWN.
- locality, admin_area, country: geographic labels with provenance/uncertainty.
- address_text: raw address as supplied/observed; not necessarily normalized.
- latitude, longitude: nullable; populate only from a traceable coordinate source.
- geometry_status: UNKNOWN, APPROXIMATE, CANDIDATE, VERIFIED.
- evidence_status: USER_REPORTED, VISUALLY_REVIEWED, INDEPENDENTLY_VERIFIED.

### pois
- poi_id: stable internal identifier for an entity candidate.
- canonical_name and raw_name: retain the working display name and original string.
- name_variants: alternate listing/sign spellings; not automatically aliases.
- category: reported category, without unsupported specificity.
- site_id: nullable link to a physical site. Multiple POIs may share one site.
- tenant_status: STANDALONE, MULTI_TENANT_MEMBER, POSSIBLE_TENANT, UNKNOWN.
- identity_status: CANDIDATE, PROBABLE, VERIFIED, UNRESOLVED, REJECTED.
- source_provenance: source type and reference for each name/category claim.

### observations
- observation_id: stable identifier for one observation event.
- poi_id and site_id: nullable links; keep unresolved entity links null.
- batch_id: original survey batch label; provenance only, never a unique entity key.
- image_ref: optional source image/frame reference; do not invent one.
- capture_date and capture_date_precision: retain date as supplied and its precision.
- observation_type: NEW_CANDIDATE, REOBSERVATION, DUPLICATE_REPLAY, CONTEXT_ONLY.
- evidence_basis: USER_DESCRIPTION, SCREENSHOT_REVIEW, INDEPENDENT_SOURCE.
- visible_text: literal reported text in the frame.
- listing_metadata: rating, review count, hours, category/status text with source/date provenance.
- notes: caveats and unresolved questions.

### relationships
Use explicit, evidence-qualified links instead of silently merging records:
- POI occupies Site.
- POI is a multi-tenant member of Site.
- Observation is a re-observation of POI.
- Two POI candidates may be possible_same_entity.
- Signage may be associated with a candidate POI.

Each relationship carries status: PROPOSED, SUPPORTED, VERIFIED, REJECTED, or UNRESOLVED, plus evidence references.

## Counting and identity rules

1. Count POI records for business/entity counts, not images, observations, pins, or batch labels.
2. Count physical sites separately. One plaza with six tenants may be one site and six POIs.
3. A new angle/date of the same POI adds an observation, not another POI.
4. A replay of the same material adds no new POI.
5. Businesses sharing a building/address remain separate POIs unless evidence shows they are the same entity.
6. Different names on a listing and building sign remain unresolved until identity is supported.
7. Temporal comparison requires a supported same-site/same-entity link and comparable physical anchors.
8. Missing coordinates, uncertain dates, incomplete addresses, and unresolved identity remain null/UNKNOWN.
9. Batch numbers are provenance only; never merge records solely because batch numbers match.
10. Ratings, hours, categories, and status are metadata, not ground truth or proof of current operation.

## Example: OASA complex

- One site record for the OASA physical complex.
- Two POI records: Respuuestos Industriales De Mexicali and Dipamex.
- Separate observation records for each business appearance.
- Two tenant-to-site relationships.
- Do not collapse the two businesses into one POI because they share a building.

## Example: Farmacias Benavides

If the 2017 and 2023 views are supported as the same branch, keep one POI/site candidate and separate observation records. The second date is not a new POI.

## Migration policy

- Preserve legacy source files unchanged until row-level migration is reviewed.
- Do not manufacture coordinates, stable IDs, image references, or VERIFIED statuses.
- Assign stable IDs only during controlled migration; retain source batch labels.
- Keep unresolved merges as candidate relationships instead of deleting either record.
- Preserve raw names and raw address strings alongside any normalized values.
- Keep source provenance and screenshot-review status for every imported observation.

## Schema files

- schemas/site.schema.json
- schemas/poi.schema.json
- schemas/observation.schema.json
- schemas/relationship.schema.json

These JSON Schemas define the target structure. They do not mean the existing master files have been converted.

**BLOON rule:** one place can host many businesses; one business can have many observations; UNKNOWN stays UNKNOWN.
