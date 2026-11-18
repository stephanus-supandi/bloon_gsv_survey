# BLOON GSV Archaeology

Forensic Street View survey of urban POIs, spatial continuity, metadata drift, and micro-economic patterns across Jakarta–Bekasi.

## Recent audit notes

- [Batches 74–77 — echo control, metadata representation, and cross-city epoch grouping (2026-11-19)](reports/batches-74-77-echo-metadata-and-cross-city-audit-2026-11-19.md) — records Batch 74 as an exact repeat of 73, Batch 75 as fresh input without a new mechanical layer, and Batches 76–77 as extensions to title/subtitle variation, background activity, metadata representation, epoch/city association, and religious-institution inventory. Camera position remains unverified; no database-failure or cross-city route claim is made.
- [Batches 61–63 — intra-panel naming, banner ambiguity, and multi-entity infrastructure representation (2026-11-18)](reports/batches-61-63-intra-panel-banner-and-infrastructure-audit-2026-11-18.md) — records title/subtitle variation within one panel, a single-pin spelling anomaly, unresolved fabric-sign boundaries, a reported musholla/SPBU multi-entity representation, and cross-field review-prose incongruence. No database corruption or camera-position claim is made.
- [Batches 58–60 — intra-render string anomaly, cross-pose panel stability, and Thamrin City name coherence (2026-11-18)](reports/batches-58-60-intra-render-and-cross-layer-audit-2026-11-18.md) — records the corrupted single-bubble text, repeated Bakso panel across different reported poses, pin-toggle/name-token extensions, and the Thamrin City token across review prose, road paint, and a POI label. No database merge, independent corroboration, or camera-position claim is made.
- [Batches 51–53 — Mas Mansyur carpet network and metadata audit (2026-11-18)](reports/batches-51-53-mas-mansyur-carpet-network-and-metadata-audit-2026-11-18.md) — records the road-plus-alley carpet-context wrinkle, relational travel-time metadata, unusual listing-hours fields, category candidates, and the continuing boundary that camera position is unverified. This is a separate batch-number sequence from the earlier San Francisco Batch 50–54 report.

- [Jatiwaringin — Jl. H. Mean Raya, Jl. Selekta, Jl. Setia 1 and Jl. Setia 1U: preliminary POI intake (2026-11-17)](reports/jatiwaringin-setia-1-setia-1u-intake-2026-11-17.md) — records user-supplied Street View summary leads as unverified candidates; keeps Nepal Van Java separate due geographic inconsistency; no coordinates, capture dates, operating-status claims, or BEO normalization are fabricated.
- [Nakula 3 — visible vehicle and unresolved business-pin context (2026-11-10)](reports/nakula-3-visible-vehicle-business-pin-context-2026-11-10.md) — records a March 2025 Street View frontage labelled “15 Jl. Nakula 3”, a white BYD-like vehicle, and an unresolved Ecosmartpool name/address lead; excludes private residence history and makes no claim of business operation, ownership, listing absence, or platform delay.
- [Batches 118–123 — Nakula, Sadewa, and Barito: repeat control and metadata audit (2026-11-10)](reports/batches-118-123-nakula-sadewa-barito-repeat-and-metadata-audit-2026-11-10.md) — records repeated content, the narrow water-refill service distinction, non-commercial neighborhood/organizational elements, pin/sign discrepancies, and strict limits on continuity, ownership, operation, and listing-date claims.
- [Batch 111 — Gang Masjid Raya: coordinate/label drift (2026-11-10)](reports/batch-111-gang-masjid-raya-coordinate-label-drift-2026-11-10.md) — zero new commodity cells; listing/pin/building mismatches and house number 36 retained as unresolved observations, with no cross-batch identity claim.
- [Batch 112 — Gang Masjid Raya: pesantren and sofa service (2026-11-10)](reports/batch-112-gang-masjid-raya-pesantren-and-sofa-service-2026-11-10.md) — zero new commodity cells; adds sofa repair as a service variant; Mahasina 4.9/262 treated as raw platform metadata.
- [Batch 113 — Essence Park: container scale (2026-11-10)](reports/batch-113-essence-park-container-scale-2026-11-10.md) — zero new commodity cells; residential complex rating and toll-road wording recorded as platform context, not evidence of gentrification.
- [Batch 114 — Masjid Raya: freight forwarding and age claims (2026-11-10)](reports/batch-114-masjid-raya-forwarding-and-age-claims-2026-11-10.md) — records an international sea/air freight-forwarding banner claim and a mosque “founded 1911” directional-sign claim, neither independently verified.
- [Kemang Raya replay audit — May 2024 vs February 2025 (2026-11-10)](reports/kemang-raya-replay-audit-may-2024-vs-february-2025-2026-11-10.md) — repeated five-frame content; zero new content-level observations; GRAMHA MUTIARA gate/security post recorded as confirmation; two capture dates kept separate with no temporal-change claim.

## Dataset

- `survey_log.csv` — 70 surveyed POIs across Blok M, Ancol, Taman Galaxy, and Kranji.
- `kranji_master_41_poi.csv` — cleaned, de-duplicated master log of 41 unique verified/observed POIs along the Pemuda Kranji corridor.
- Observation dates/capture labels are recorded as supplied by the survey log.
- The Kranji master merges repeated appearances of the same POI while retaining distinct visually verified adjacent nodes.
- This repository is a working research dataset, not a claim of legal property boundaries or business ownership.

## Method

The survey distinguishes:

1. **Observation / FACT** — what is visibly present in the frame.
2. **Spatial identity / MATCH** — whether physical objects or spatial units can be linked.
3. **Change detection** — reserved for explicitly authorized cross-date comparisons with sufficient evidence.
4. **Inference / HYPOTHESIS** — interpretations that remain testable rather than established facts.
5. **UNKNOWN** — unresolved cases are retained rather than forced into an identity.

### Evidence hierarchy

Physical evidence such as permanent signage, address plates, road-name paint, fixed infrastructure, geometry, fences, gates, and building relationships is preferred over Google Maps labels.

Map/business labels are treated as **metadata**, not ground truth.

A readable token alone does not establish object, property, business, or cross-date identity.

### Kranji Ronde 8 notes

The Jan 2026 Kranji batch adds a new cell-phone retail row around Hallo Phone, Asia Afrika, and Happy Cell, with vivo/oppo/itel/Samsung promotional signage and repeated transient scene elements used only as capture-continuity clues.

A separate Apr 2025 observation records Toko Giat Makmur with a visible bulk banana display, treated as an observed wholesale/agricultural-supply node rather than an inferred property or market boundary.

The Ronde 8 interpretation of smartphone-retail clustering and Pasar Kranji spill-over remains an analytical hypothesis supported by observed co-location, not a causal economic claim.

## Current survey scope

- **Blok M** — commercial, transit, retail, F&B and institutional nodes.
- **Ancol** — arts, craft, gallery, market and tourism-related nodes.
- **Taman Galaxy** — residential and neighborhood-retail observations.
- **Kranji** — micro-medical, micro-fintech, F&B, retail, construction-materials and traditional-market nodes.

## Important caveat

Street View imagery and platform metadata are subject to their respective copyrights and terms of use. This repository records observations and analysis; it does not redistribute Google's Street View imagery.

## Status

Working research dataset. Future additions should preserve provenance and uncertainty rather than silently rewriting earlier observations.

## Suggested citation

**BLOON GSV Archaeology — Jakarta–Bekasi Survey Log, 2026.**  
Repository: `stephanus-supandi/bloon_gsv_survey`
