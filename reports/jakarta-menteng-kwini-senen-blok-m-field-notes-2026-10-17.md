# BLOON GSV Archaeology — Jakarta Urban POI Field Notes

- **Record prepared:** 2026-10-17
- **Survey areas:** Menteng; Dr. Abdul Rahman Saleh / Kwini / Senen; Blok M / Falatehan
- **Input:** User-supplied field notes and descriptions of map/Street View screenshots
- **Status:** Preliminary transcription and research index — **not independently verified**
- **Evidence files:** Original screenshots and image metadata were not attached to this report

## Purpose and evidence limits

This report preserves candidate place names and observations from the survey session so they can be checked later. It does not claim that every map label is correct, that businesses occupy the same premises across dates, or that proximity proves ownership, affiliation, or a business succession.

The place names below are transcribed from user-supplied notes. They have not been independently checked against current Google Maps listings, historical Street View captures, business registries, or official address records in this commit.

## 1. Menteng / Taman Suropati area

Candidate anchors and labels mentioned in the field notes:

- Taman Suropati
- Jalan Besuki
- SDN Menteng 01
- Jalan Teuku Umar

### Verification tasks

1. Record the exact Street View capture date and viewpoint for each frame.
2. Confirm road names and school identity from visible permanent signage or authoritative records.
3. Keep the identity of a building separate from a map pin or business label.
4. Do not infer a route, adjacency, or property boundary from the order in which screenshots were reviewed.

## 2. Dr. Abdul Rahman Saleh / Kwini / Senen area

Candidate anchors and labels mentioned in the field notes:

- Jalan Dr. Abdul Rahman Saleh
- RSPAD Gatot Soebroto
- Jalan Kwini / H. Imam Sapi'ie
- BRI KCP RSPAD
- Pegadaian
- Atrium Senen
- Millennium Mall
- Lumire Hotel
- Doctors Yanti Silman

These are a **candidate list**, not a verified spatial inventory. In particular, the spelling and exact identity of “Doctors Yanti Silman” should be rechecked against the original screenshot or a reliable public listing rather than silently normalized.

### Verification tasks

- Capture exact label text, source, URL or screenshot identifier, and capture date.
- Geolocate each candidate independently before creating spatial edges.
- Distinguish a business label from physical signage visible in imagery.
- Treat shared road names or apparent proximity as clues only until the relevant viewpoint and coordinates are established.

## 3. Blok M / Jalan Falatehan area

Candidate labels and scene notes mentioned in the field notes:

- Sotis Hotel
- 38 Prima Hotel
- PT Asuransi Tri Pakarta
- BNI ATM
- DJODY Gallery / Circle K
- Bella Furniture
- DOMUS Group
- Triple Nine 999
- An's Place bar — described in the notes as an older pin marked closed
- “Obama Fans Club” — described in the notes as a label appearing in a later map view near a red-and-white facade

The descriptions above record what the notes reported; they do not independently establish current business status, exact premises, or historical continuity.

### Special handling: “Obama Fans Club”

The name “Obama Fans Club” is recorded as a **reported map label only**. Its presence does not establish an affiliation with Barack Obama, a school, an organization, a property owner, or another similarly named entity. The apparent relationship to the red-and-white facade requires direct evidence from the original frame and a dated source.

### Special handling: older and newer business labels

The note that an older An's Place pin was marked closed, alongside another label in the area, is not enough to conclude that one business replaced another. A defensible change-detection record needs at least two dated observations, comparable viewpoints or coordinates, and evidence tying each label to the same physical premises.

## 4. Duplicate screenshots and batch accounting

The user reported that four of five images in one batch were duplicate Bekasi map screenshots, while one image introduced a new “Obama Fans Club” map-label candidate.

This is a **user-reported batch summary**, not an independently re-counted image audit: the five source images were not attached to this report. Do not add five new POIs on the basis of the image count. A duplicate screenshot is not a new spatial observation unless it contributes distinct evidence, such as a different date, viewpoint, zoom level, or label state.

## 5. Evidence model

Use the repository's existing evidence vocabulary:

| Class | Meaning for this report |
|---|---|
| OBSERVATION | A feature or text directly visible in a retained source image, with the image/viewpoint identified |
| LABEL | Text supplied by a map or business listing; metadata, not ground truth |
| MATCH | A candidate identity link supported by distinctive physical or documentary evidence |
| CHANGE_CANDIDATE | A possible difference between dated observations, pending comparable evidence |
| HYPOTHESIS | An interpretation that remains testable and must not be presented as fact |
| UNKNOWN | Missing, ambiguous, or contradictory evidence retained without guessing |

For every future row, record: candidate ID, exact label/transcription, source URL or screenshot ID, capture date if known, observation date, viewpoint or coordinates if available, evidence class, confidence rationale, and unresolved questions.

## 6. Claims deliberately not made

This report does **not** conclude that:

- any listed business is currently open or operating at the stated premises;
- one business replaced, owned, or was affiliated with another;
- “Obama Fans Club” is affiliated with Obama, a school, or any other organization;
- a map label proves that a business existed on the date of the imagery;
- visual adjacency establishes a legal property boundary or ownership;
- the user-reported duplicate count has been independently verified.

## 7. Next verification checklist

- [ ] Attach or identify the original screenshots in a local evidence log; do not redistribute copyrighted Street View imagery in this repository.
- [ ] Transcribe exact labels and note any OCR or reading uncertainty.
- [ ] Record source capture dates separately from the date the survey was performed.
- [ ] Check each candidate's coordinates and viewpoint before asserting spatial adjacency.
- [ ] Compare older and newer imagery only when dates and locations are sufficiently comparable.
- [ ] Update the master CSV only after assigning stable candidate IDs and preserving uncertainty.
- [ ] Record contrary evidence as well as confirming evidence.

## Provenance note

This file is a structured record of user-supplied field notes prepared on 2026-10-17. Because the underlying screenshots were not included, all named places and batch observations remain provisional until the source material is attached or referenced and checked.

Repository: [BLOON GSV Archaeology](https://github.com/stephanus-supandi/bloon_gsv_survey)
