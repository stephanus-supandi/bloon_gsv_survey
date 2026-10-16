# BLOON GSV Archaeology — South Bekasi Macro Spatial Context

- **Batch:** South Bekasi — Macro Spatial Context
- **Map/screenshot reference date:** March 2025 (as reported by the source notes)
- **Record prepared:** 2026-10-17
- **Project:** [BLOON GSV Survey](https://github.com/stephanus-supandi/bloon_gsv_survey)
- **Status:** Preliminary context layer — **not a verified GIS dataset**

## Purpose

This note records a macro-level interpretation of a user-provided map screenshot to help organize the BLOON GSV Archaeology survey. It is a working index for later checks against administrative boundaries, road geometry, Street View imagery, and reliable public sources.

The screenshot itself and the original image metadata are not included in this commit. Place names read from the screenshot are therefore recorded as observations from the supplied notes, not independently reproduced observations.

## 1. Administrative context

Bekasi Selatan is an administrative **kecamatan** within Kota Bekasi, West Java. BPS's *Kecamatan Bekasi Selatan Dalam Angka 2024* reports a total area of **15.81 km²** and lists five kelurahan:

- Jaka Mulya
- Jaka Setia
- Pekayon Jaya
- Marga Jaya
- Kayuringin Jaya

The reported mid-2023 population of **214,493** appears in the secondary South Bekasi summary on Wikipedia. Treat this figure as a reported estimate pending direct extraction and citation to the corresponding official BPS table.

**Important:** The administrative fact that Jaka Setia belongs to Bekasi Selatan does not prove that every road or point of interest mentioned in the working notes belongs to the same kecamatan. Each location must be checked against its actual coordinates and the administrative boundary.

## 2. Macro anchors noted from the map

These names were transcribed from the working report/screenshot notes and are **candidate anchors**, not yet a validated POI inventory:

- Jalan Bulian I
- Jalan Matahari II / Taman Galaxy area
- Jalan Bintang Raya
- Jalan Insinyur H. Juanda
- Jalan Pantura
- Galaxy Space
- Cikunir Raya
- Jalan Rajawali
- Jalan Garuda
- Jalan Cendrawasih
- Nakula 3
- Jalan Permata
- Jalan Batu Mulia

For each candidate, capture coordinates, source imagery/date, exact displayed name, kelurahan/kecamatan, and verification status before adding it as a confirmed graph node.

### Preliminary spatial hypotheses

- The Taman Galaxy / Jalan Matahari / Nakula cluster may provide a useful local-scale survey area.
- Cikunir Raya and the MBZ elevated toll corridor are regional infrastructure anchors worth comparing with the local road network.
- The grouping of all named places into Bekasi Selatan remains **unverified**. In particular, Jalan Ir. H. Juanda is associated with locations in Bekasi Timur in some municipal contexts; the exact segment referenced by the screenshot must be established before assigning its administrative unit.
- The name “Jalan Pantura” is ambiguous without coordinates or a nearby landmark.

## 3. MBZ elevated toll road

The official BPJT overview states that the elevated Jakarta–Cikampek II toll road, later named **Jalan Layang MBZ Sheikh Mohamed Bin Zayed**, extends approximately **36.84 km** from Junction Cikunir to Karawang Barat.

The name was described by BPJT as an honour to the United Arab Emirates in the context of Indonesia–UAE diplomatic relations. **The name alone is not evidence that the UAE financed the project.** Financing, ownership, construction contracts, and naming rationale are separate questions and require separate sources.

Do not infer that the elevated toll road crosses the whole Bekasi Selatan district just because it appears diagonally on a zoomed-out map. Confirm the alignment, ramps, and local-road connections using authoritative maps.

## 4. POIs requiring name verification

The following labels were reported as partially read or seen in the map interface:

| Candidate label | Current status | Required check |
|---|---|---|
| Galaxy Space | Unverified candidate | Confirm exact name, coordinates, and business type |
| Bullshirt Store | Unverified candidate; “recently viewed” UI may be personal interface state | Confirm whether it is a real mapped POI and capture its map source |
| Nasi Goreng Mas… | Incomplete label | Do not expand the name by guessing; inspect the original screenshot or listing |
| RAYA CH… | Incomplete label | Do not assume “Raya Chicken” or another business without evidence |

UI labels such as “recently viewed” may reflect account-specific browsing history rather than an objective property of the place.

## 5. Population and density calculation

Using the reported values:

- Area: 15.81 km²
- Mid-2023 population estimate: 214,493
- Approximate density: 214,493 / 15.81 = **13,567 people/km²** (rounded)

The calculation is reproducible, but the population figure should be cited to the official statistical table before treating it as a final authoritative figure. High density alone does not establish that Bekasi Selatan is a “city within a city”; that phrase is an interpretation, not an administrative classification.

## 6. Provisional graph delta

Suggested nodes, pending validation:

- `admin:bekasi-selatan` — administrative district; area 15.81 km² (BPS 2024)
- `infra:mbz-elevated` — elevated toll corridor; route overview from BPJT
- `road:cikunir-raya` — candidate road anchor
- Candidate local-road and POI nodes listed above

Suggested edge types:

- `CONTAINS`: administrative boundary relation, only after coordinates/boundaries confirm it
- `CONNECTS_TO`: road-network connection, only after route geometry confirms it
- `OBSERVED_NEAR`: proximity based on a cited map/Street View observation
- `POSSIBLE_MATCH`: uncertain POI/name match
- `CONTRADICTS`: evidence that challenges an earlier assignment

Do not create a `CONTAINS` edge merely because a label appears in the same screenshot.

## 7. Unknowns and next verification tests

1. Is the exact Jalan Pantura segment inside Bekasi Selatan, on a boundary, or elsewhere?
2. What are the complete names and coordinates for “Nasi Goreng Mas…” and “RAYA CH…”?
3. What is the actual road-access relationship between Jalan Bulian I and the MBZ toll ramps?
4. Which KRL, LRT, TransJakarta, or other transit stops are geographically relevant to the candidate survey area?
5. Which specific road segments and POIs belong to each of the five kelurahan?
6. Does the source screenshot show the same map date and labels as the March 2025 batch description?

### Acceptance criteria for promoting a candidate to verified

- Exact coordinate or sufficiently precise address captured.
- Source URL and retrieval/imagery date recorded.
- Administrative assignment checked against an authoritative boundary/source.
- Name copied exactly as displayed; ambiguous labels stay ambiguous.
- At least one independent corroborating source where practical.
- Status is explicit: `NOT_CHECKED`, `CANDIDATE`, `PARTIALLY_VERIFIED`, or `VERIFIED`.

## 8. Source register

1. **Badan Pusat Statistik Kota Bekasi**, *Kecamatan Bekasi Selatan Dalam Angka 2024* (official publication, released 26 September 2024):  
   https://bekasikota.bps.go.id/id/publication/2024/09/26/ae6a183156c51d7de171668e/kecamatan-bekasi-selatan-dalam-angka-2024.html

2. **BPJT**, *Sederet Fakta dan Asal Nama Jalan Layang MBZ Sheikh Mohammed Bin Zayed* (24 February 2023):  
   https://bpjt.pu.go.id/sederet-fakta-dan-asal-nama-jalan-layang-mbz-sheikh-mohammed-bin-zayed/

3. **Wikipedia**, *South Bekasi* (secondary summary; use as a discovery aid, not as the sole authority for official statistics):  
   https://en.wikipedia.org/wiki/South_Bekasi

## Audit note

This file intentionally downgrades the original report's “VERY HIGH” confidence to **preliminary / mixed confidence**. The administrative area and MBZ corridor have authoritative reference sources; the full POI list, road topology, screenshot interpretation, and claim that all explored places lie within Bekasi Selatan remain unverified.

No claim is made that a GIS boundary overlay, coordinate validation, Street View comparison, or field survey has been performed.
