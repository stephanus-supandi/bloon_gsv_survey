# BLOON GSV Archaeology

Forensic Street View survey of urban POIs, spatial continuity, metadata drift, and micro-economic patterns across Jakarta–Bekasi.

## Dataset

- `survey_log.csv` — 70 surveyed POIs across Blok M, Ancol, Taman Galaxy, and Kranji.
- Observation dates/capture labels are recorded as supplied by the survey log.
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
