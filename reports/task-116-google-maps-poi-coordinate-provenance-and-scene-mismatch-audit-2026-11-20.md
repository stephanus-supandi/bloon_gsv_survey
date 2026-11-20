# BLOON GSV — Task 116
## Google Maps POI–Scene Mismatch, Pin Placement, and Coordinate Provenance Audit

**Date:** 2026-11-20  
**Project:** BLOON_GSV_SURVEY  
**Inputs:** Qwen Task 116A; Gemini Task 116B; editorial/technical review  
**Status:** Methodology baseline; no individual Google Maps POI has been verified as misplaced by this report.

## 1. Executive summary

Task 116 opens a research track beyond Street View scene inventory: the relationship between a Google Maps place identity (POI), its displayed pin, the physical scene, and the provenance of the underlying location data.

The two submissions are complementary:

- **Qwen** proposes a POI–scene mismatch taxonomy, confidence tiers, a decision tree, and structured audit fields.
- **Gemini** maps documented contribution and business-profile pathways, geocoding concepts, Place IDs, content-partner data, and the limits of publicly visible provenance.

The combined result is suitable as a methodology baseline, subject to the corrections in this report. It is not evidence that any particular pin was deliberately manipulated, incorrectly submitted, or placed at a wrong coordinate.

## 2. Four layers that must remain separate

Every case should be assessed across four distinct layers:

1. **POI identity** — name, category, business/place identity, possible aliases or duplicates.
2. **Coordinate placement** — the geographic point represented by the pin, and its relationship to a building, parcel, entrance, access point, or street.
3. **Scene correspondence** — whether visible signage, building use, and scene details appear consistent with the selected POI.
4. **Provenance and verification** — who or what supplied the record/coordinate, when it was changed, and what evidence was used to review it.

A mismatch in one layer does not establish a mismatch in the others. A correct business identity can have an imprecise pin; a correctly placed pin can have stale business attributes; and a pin that appears to sit on a pole in a perspective image may be geographically located elsewhere.

## 3. Qwen taxonomy — accepted as candidate codes

The following codes are retained as overlapping anomaly tags, not mutually exclusive diagnoses.

| Code | Working label | Operational observation |
|---|---|---|
| HCP | House-with-Commercial-Pin | A residential-looking structure is associated with a commercial POI. |
| EBP | Empty/Inactive-looking Scene with POI | The scene appears closed, vacant, or inactive at the imagery moment while a POI is displayed. |
| KCD | Residential-looking Scene / Category Difference | A residential- or boarding-house-looking structure is associated with a category that appears functionally different. |
| MFP | Multi-pin Facade | Multiple POIs appear associated with one apparent facade or structure. |
| NPA | Neighbor/Road/Object Pin Appearance | The displayed pin appears, from the observed view, to fall on a neighboring structure, road, pole, median, or other non-business object. |
| FCS | Possible Function-Change / Stale Listing | Physical signage or apparent use differs from the selected POI identity. |
| NSG | No Signage Visible | No relevant business signage is visible from the observed viewpoint. |
| MNI | Multiple Names / Identity Ambiguity | Different POI names or categories appear to refer to one apparent place or coordinate. |

### Taxonomy cautions

- Codes may co-occur. For example, HCP + NSG or MFP + MNI may describe the same case from different angles.
- These codes identify an **observed mismatch pattern or question**, not a proven database error.
- “Empty” must describe only the visible imagery moment. Prefer the neutral phrase **empty/inactive-looking scene** over a claim that the property is actually vacant.
- A house can legitimately host a registered home business; an online/service-area business may not serve customers at its registered address.
- No visible sign does not establish that no business exists. The sign may be on another side, inside, temporary, absent by design, or not visible in the selected frame.
- Multiple pins on one facade may represent tenants, floors, departments, practitioners, entrances, aliases, stale records, duplicates, or pin-placement issues. The scene alone may not distinguish them.
- A category difference is not automatically “category drift”; actual use and listing history are needed to establish change over time.
- A pin that visually overlaps a pole or roof in Street View is not enough to establish its latitude/longitude is on that object. Perspective and projection must be ruled out.

## 4. Confidence tiers — corrected rule

Qwen's tiers are useful, but its examples contain an important ambiguity: it suggests non-adjacent Street View captures may support VERIFIED, while also requiring evidence outside Street View. These conditions conflict.

For this project, apply the following rule:

| Tier | Required basis | What it does not mean |
|---|---|---|
| **OBSERVED** | A directly visible property of the supplied frame or map view, described without inference. | Does not establish an error. |
| **SUSPECTED** | The observation is consistent with a named mismatch hypothesis, but plausible alternatives remain. | Does not establish that the POI or coordinate is wrong. |
| **SUPPORTED** | Multiple materially distinct evidence sources support the same bounded hypothesis; their provenance and dependencies are recorded, and obvious alternatives have been tested. | Multiple screenshots, nearby frames, or repeated renderings from one underlying source do not automatically count as independent evidence. |
| **VERIFIED** | The specific claim is confirmed by suitable independent ground truth, such as a field survey tied to a known coordinate/reference system, authoritative address/parcel data, operator confirmation, or equivalent evidence. | Repeated Street View imagery alone does not establish VERIFIED. |
| **UNRESOLVED** | Evidence is insufficient, the pin/scene cannot be associated reliably, or competing explanations cannot be separated. | Is not a negative finding. |

**Hard rule:** Street View-only material may document observations and support hypotheses, but it does not by itself verify the real-world correctness of a POI coordinate. Multiple Street View dates can help assess visual consistency or change, but they remain imagery evidence and must not be promoted to independent ground truth.

The word **SUPPORTED** must be accompanied by an evidence-dependency note: source type, capture/date, whether it derives from the same underlying dataset, and what alternative explanations remain open.

## 5. Decision workflow

For each candidate case:

1. **Identify the object being assessed.** Record the selected POI, displayed pin, map view, Street View view, and whether the pin is actually visible. If the pin is not visible or cannot be associated with the scene, mark UNRESOLVED for pin placement.
2. **Separate identity from placement.** Record POI name/category separately from the apparent physical structure and apparent pin position.
3. **Describe the scene literally.** Examples: “residential-looking facade”; “shutter closed in this imagery”; “no sign visible from this viewpoint”; “three POI labels appear associated with one facade.” Avoid “fake business,” “vacant property,” or “wrong coordinate” as initial observations.
4. **Apply one or more candidate codes.** Record why each applies and list benign alternatives.
5. **Test projection and viewpoint.** Do not infer geographic placement from apparent overlap in a perspective Street View frame. Use map geometry, additional viewpoints, and independent coordinate references where available.
6. **Assess evidence independence.** Repeated panels, adjacent captures, same-source imagery, or replayed screenshots are not independent corroboration merely because they are repeated.
7. **Assign a tier and list missing evidence.** Do not promote a case solely because several weak indicators point in the same direction.

## 6. Google Maps data pathways — working technical model

Gemini identifies several documented or plausible pathways relevant to POI records:

### 6.1 Business Profile

Business owners/managers can manage business information, including an address and map marker position. Google documentation describes adjusting a location pin where the address cannot be found or is not positioned correctly.

Business Profile verification concerns a business's eligibility/control and profile management. It must not be treated as a guarantee that every coordinate is survey-grade or correctly located at the building entrance.

Google's representation guidelines distinguish customer-facing storefronts from service-area businesses. Eligibility and address-display rules depend on the business model; do not infer a violation from a residential-looking facade alone.

### 6.2 User contributions

Google Maps users can suggest missing places and edits. These are contribution pathways, not proof that a suggested record was accepted without review or that the contributor personally surveyed the coordinate.

A contributor's own contribution history is not equivalent to a complete public audit log for every POI.

### 6.3 Geocoding

Geocoding converts addresses to geographic coordinates and can return a result classification such as ROOFTOP, RANGE_INTERPOLATED, GEOMETRIC_CENTER, or APPROXIMATE in the relevant Geocoding API response.

**Critical limitation:** These location_type values describe a geocoding result. They are not a publicly exposed accuracy grade for every consumer Google Maps POI pin, and they do not prove the pin shown in a Street View screenshot was generated by that particular geocoding result.

### 6.4 Places API and Place IDs

Places API provides programmatic place search/details and place identifiers. A Place ID is an identifier, not a coordinate and not proof of a physical survey. Google documentation notes that Place IDs can change and that a place may have more than one Place ID in some circumstances.

Do not infer that a Place ID change necessarily means a business moved, its coordinate changed, or the physical entity changed.

### 6.5 Content partners and authoritative datasets

Google Maps Content Partners is a relevant potential pathway for organizations that supply geospatial content. The exact accepted data types, file formats, schemas, eligibility rules, and review requirements must be checked against current partner documentation before being treated as a precise technical specification.

The existence of a partner data pathway does not show that any specific POI in this survey came from a partner dataset.

### 6.6 Other potential data and maintenance processes

Google may combine, review, update, or reconcile information from different sources. The precise internal weighting, matching, conflict-resolution, and per-POI provenance history are not established by the public documentation listed here. Treat detailed descriptions of those internal mechanisms as unknown unless a source explicitly documents them.

## 7. Provenance questions and public visibility

The research question is not only “who can add a pin?” but also “what can an external investigator know about this specific pin?”

| Question | Current audit position |
|---|---|
| Can a business manager adjust a Business Profile marker? | Documented capability, subject to applicable workflow and eligibility. |
| Can a Maps user suggest a place or edit? | Documented contribution pathway. |
| Can geocoding produce different precision classes? | Documented for relevant API geocoding responses. |
| Does a visible pin prove Business Profile verification? | No. |
| Does profile verification prove coordinate accuracy? | No. |
| Can a public investigator see a complete per-POI creator/change history? | No such complete public provenance log has been identified in this review. |
| Can a public investigator know the original coordinate source for an arbitrary POI? | Not from the visible pin alone; source-specific provenance remains unknown. |
| Can a public investigator infer a POI's exact positional error in metres from the displayed marker? | Not reliably without an independent reference coordinate and a defined measurement method. |

This is a statement about the limits of the public material reviewed, not a claim that Google has no internal logs.

## 8. Candidate mismatch mechanisms

The following are hypotheses to test, not diagnoses:

- Ambiguous or incomplete address geocoding.
- Manual pin placement that is approximate or incorrect.
- Stale business information after closure, relocation, or rebranding.
- Duplicate, overlapping, or aliased POI records.
- Multi-tenant buildings with multiple valid businesses or entrances.
- Residential address used for a business or service-area operation.
- Building-footprint point versus customer entrance/access-point difference.
- Map/Street View perspective or 3D rendering that makes a pin appear to overlap the wrong object.
- Incomplete or inconsistent source datasets and subsequent reconciliation.

No one mechanism should be assigned to an individual case without evidence that discriminates it from alternatives.

## 9. Suggested audit schema

CSV fields:

    case_id,observation_date,imagery_date,zone,poi_name,poi_category,place_id_if_available,pin_visible,displayed_pin_relation,apparent_structure,scene_condition,signage_match,anomaly_codes,confidence_tier,evidence_sources,evidence_dependencies,benign_alternatives,missing_evidence,independent_reference,notes

Illustrative JSON object (not a real case):

    {
      "case_id": "CASE-001",
      "poi_name": null,
      "poi_category": null,
      "place_id_if_available": null,
      "pin_visible": null,
      "displayed_pin_relation": "unresolved",
      "apparent_structure": "residential-looking",
      "scene_condition": "no_business_signage_visible_from_this_view",
      "signage_match": "unknown",
      "anomaly_codes": ["HCP", "NSG"],
      "confidence_tier": "SUSPECTED",
      "evidence_sources": [],
      "evidence_dependencies": [],
      "benign_alternatives": [
        "legitimate_home_business",
        "service_area_business",
        "signage_not_visible_from_viewpoint"
      ],
      "missing_evidence": [
        "independent_address_or_parcel_reference",
        "operator_confirmation",
        "coordinate_validation"
      ],
      "verified": false,
      "notes": "Illustrative schema only; not a real case."
    }

Do not create fake example coordinates, owners, businesses, capture dates, or field results. Empty/null values are preferable to invented data.

## 10. Source register supplied for follow-up verification

The following URLs were supplied in the Gemini research output. They are retained as a source-check list; their inclusion here does not mean every page, claim, current policy detail, or API field has been independently revalidated in this audit.

- Google Business Profile Help — Manage your business address: https://support.google.com/business/answer/2853879?hl=en-US
- Google Business Profile Help — Guidelines for representing your business on Google: https://support.google.com/business/answer/3038177?hl=en-US
- Google Business Profile Help — Verify your business with a video recording: https://support.google.com/business/answer/14271705?hl=en-US
- Google Business Profile APIs — VerificationMethod: https://developers.google.com/my-business/reference/verifications/rest/v1/VerificationMethod
- Google Maps Help — Add a missing place: https://support.google.com/maps/answer/6320846?hl=en-US
- Google Maps Help — Edit place information: https://support.google.com/maps/answer/7084895?hl=en-US
- Google Maps Platform — Geocoding API: https://developers.google.com/maps/documentation/geocoding
- Google Maps Platform — Geocoding API overview: https://developers.google.com/maps/documentation/geocoding/guides-v3/overview
- Google Maps Platform — Geocoding service and location types: https://developers.google.com/maps/documentation/javascript/geocoding
- Google Maps Platform — Places API overview: https://developers.google.com/maps/documentation/places/web-service/overview
- Google Maps Platform — Place IDs: https://developers.google.com/maps/documentation/places/web-service/place-id
- Google Maps Content Partners: https://contentpartners.maps.google.com/
- Google Maps Content Partners requirements: https://support.google.com/mapcontentpartners/answer/144284?hl=en-US

## 11. Explicit exclusions and privacy boundary

This report does not include internal investigative scripts, crawlers, endpoint probes, account-specific tools, private datasets, credentials, or unpublished code. Such tools belong in a controlled local/private workspace unless there is a deliberate decision to publish a safe, documented, reusable component.

This report does not identify private residents, infer property ownership, or treat a residential-looking building as suspicious by itself. It does not redistribute Street View imagery.

## 12. Current conclusion

Task 116 establishes a disciplined framework for investigating POI identity, coordinate placement, scene correspondence, and provenance separately. Qwen's taxonomy is retained as a set of candidate observation codes. Gemini's source-path model is retained with important distinctions between Business Profile verification, geocoding result types, Places identifiers, and actual coordinate accuracy.

No specific POI has been verified as misplaced. No pin creator, original coordinate source, or internal Google review history has been identified. The next step is to apply this framework to carefully selected examples with independent reference evidence, not to label all unusual pins as errors.

**Principle: GOBLOK BOLEH. NGARANG JANGAN.**
