# BLOON GSV Survey — Batches 58–60: Intra-render String Damage, Cross-pose Panel Stability, and Thamrin City Name Coherence

**Date recorded:** 2026-11-18  
**Repository:** `stephanus-supandi/bloon_gsv_survey`  
**Method principle:** GOBLOK BOLEH. NGARANG JANGAN.

> **Sequence note:** Batch numbers are local to this visual-audit sequence. They are not the earlier San Francisco Batch 50–54 sequence or other repository batch series.

## Scope and provenance

This report records the observer's descriptions and interpretations of Batches 58–60. The original Street View frames were not independently re-inspected for this update. Frame contents, pin labels, panel values, Chrome timestamps, battery values, and UI glyphs are therefore **user-reported observations**, not independent image verification.

The audit keeps physical scene descriptions, road paint, Google POI/panel data, review prose, and viewer/device chrome in separate evidence classes. No reported layer independently verifies the camera's exact position.

## Batch 58 — Intra-bubble string corruption and cross-pose panel stability

### Wrinkle 1: corrupted text within one pin bubble

Frame f3 is reported to show a single pin bubble whose text reads approximately:

`Bubur ayam Bang Olil =====(Bubur bang ECO...`

The delimiter-like `=====`, unmatched opening parenthesis, and concatenation of two apparent name strings make this different from earlier name-churn cases involving separate renders or labels. Here, the reported anomaly is **within one rendered bubble**.

The cause is unresolved. Possibilities include a long/truncated business name, overlapping entity text, or a rendering/data-display defect. The string alone does not establish that two database entities were merged, that a database record is structurally corrupted, or that the underlying business count is wrong.

**Classification:** user-reported intra-render string anomaly; cause unknown. It extends the name-churn observation family to the string level inside one render, without establishing an entity-count or database-merge failure.

### Wrinkle 2: same POI panel across two different poses in one batch

The observer reports that f1 and f5 show substantially different scene poses:

- f1: central trembesi tree, silver Innova, CIMOL cart, and traffic light.
- f5: black SUV in front, Bluebird taxi, Yakult cart, and a `DISEWA KAN LANTAI 2` banner.

Despite those different reported scene compositions, both frames show the pin **“Bakso Rusuk Samanhudi Tanah Abang”** with an identical panel:

- rating/review count: **4.7 (2052)**
- category: **Bakso restaurant**
- price: **Rp 25–50K**
- hours: **Open 24 hours**

This is an intra-batch, cross-pose repeat of the same reported panel fields. It supports the narrow description that the displayed panel is stable across the two reported views. It does not independently establish why the panel is stable, whether the underlying record is correct, whether both views map to the same physical frontage, or where either camera pose is located.

### Other observations retained as extensions

- “Samanhudi Tanah Abang” is a market/place-name token in a business label; it is homonym-prone and is not a camera anchor.
- “Bang Olil” is a personal-name style token in a food-business label; it does not identify a unique business without independent evidence.
- The reported `Rp 25–50K`, `Open 24 hours`, and 2052-review fields remain platform metadata. Price, hours, and popularity do not provide coordinates.
- **Mess Kowal Cut Nyak Dien** is described as a repeat/scrub-back from an earlier batch; it is not promoted as a new spatial finding.
- Road-name paint reported as `Jl. K.H. Mas Mansyur` and `Jl. Cosmo Ter...` is retained as visible text, not a lens fix.
- A physical Indonesian flag, a large white building without readable signage, and carts/vehicles are scene observations only. No institutional identity is inferred from the building.
- A second Bubur ayam panel is reported without a corresponding pin bubble in the canvas; this remains a panel/pin presentation difference, not proof of a missing or duplicated entity.
- Companion glyphs (ATOM, blue lock, orange mirror, grey pin) are viewer-interface artifacts, not geographic evidence.
- Chrome is reported as May 2025 on all five tiles; the displayed clock is 2:27 throughout; battery changes from 96% to 97%. These are viewer/device values, not camera telemetry.

**Batch assessment:** Filling, with two thin mechanical observations: intra-bubble string corruption and same-panel recurrence across two different reported poses. Neither establishes a database merge, entity count, or camera position.

## Batch 59 — Name and language tokens; repeated two-pin toggles

The observer reports two separate two-pin toggles:

- f1/f2: **ATM BCA 5.0 (1)** ↔ **Indomaret Mas Mansyur 2 3.7 (94)**, with the scene described as pixel-identical.
- f4/f5: **Warung Sembako RIJAL MADURA** ↔ **An Nur**, also with the scene described as pixel-identical.

These are retained as repeated examples of pin/listing toggling over a reported unchanged pose. They do not establish camera movement, physical adjacency, or identity between the selected POIs.

### Two small name/language observations

- **An Nur** is also the name of a Quranic surah. Its use as a business name extends the observed set of Arabic/religious vocabulary in business-name tokens. The name is common and homonym-prone; it does not establish the owner's intention, religious identity, affiliation, or the religious character of the surrounding area.
- **RIJAL MADURA** and the accompanying phrase reported as `Ta'tao K Pesse` are retained as regional/language tokens. The phrase's meaning is unresolved here; no translation, language identification beyond the observer's tentative Madura association, or cultural inference is asserted.

### Other observations retained briefly

- **KLINIK PRATAMA CITRA MEDIKA** is reported as a healthcare-institution listing/name. The name alone does not identify a unique clinic or verify its operation.
- A banner reads `SUPER GADAI TANPA BIAYA ADMIN TANPA POTONGAN BUNGA`; this is an advertising claim on a banner, not an independently verified service/fee condition.
- Road paint is reported as `JL. K.H. MAS MANSYUR NO. 66`. The number is retained as a visible text token, not a verified address-to-camera match.
- A displayed `53 min` value remains relational/platform metadata; it is not a radius, distance, or coordinate.
- Companion glyphs (orange fork, blue lock, ATOM, grey pin) remain viewer-interface artifacts.
- Chrome is reported as May 2025 throughout; the displayed clock changes from 2:27 to 2:26; battery remains 97%. No camera-session conclusion is drawn from these values.

**Batch assessment:** Filling / extend-verify. No new mechanical evidence class is claimed. The surah-name and regional-language tokens are retained as small descriptive observations, not new identifiers or geographic proof.

## Batch 60 — One place-name across review prose, road paint, and POI listing

### Cross-layer name coherence

The observer connects three appearances of the same name token:

1. **Batch 57 review prose:** “Thamrin City” in the reported Hotel Caravan review panel.
2. **Batch 60 road paint:** `Jl. Cosmo Terrace Thamrin City` in f4/f5.
3. **Batch 60 POI pin:** `Soto Ayam Thamrin City` in f4.

This is a useful cross-layer consistency observation: one place-name appears in review prose, physical road-paint text, and a POI label across the referenced batches.

It is not three independent geospatial confirmations. The sources may be dependent, copied, or otherwise related; that dependency has not been tested. Even a coherent place-name across several self-reported layers does not establish that the camera stood at Thamrin City or that the selected POI is physically at the camera position.

This mechanism is distinct from the earlier multi-record/name-churn cases: those concern one apparent entity represented by multiple labels/records, whereas this observation concerns one name token recurring across different representational layers. It is also the inverse descriptive pattern of a one-entity/many-label fracture: here the token is consistent, but its geographic referent remains unverified.

### Other observations retained briefly

- **Rm Junjung Sirih** is retained as a regional/Minang-style name token; it is homonym-prone and not a unique geographic identifier.
- A **SUPER GADAI** banner reportedly includes `OJK TERDAFTAR DAN DIAWASI`. This is a printed regulatory claim, not independent verification of registration or oversight.
- Road paint is reported as `JL. K.H. MAS MANSYUR NO. 66`, extending the recurring road-name/house-number text observations without proving the camera's address.
- f2/f3 reportedly toggle between **Sop Kaki Sapi “Setia”** and **Indomaret Mas Mansyur 2** over a pixel-identical pose. This extends the two-pin toggle family.
- f4/f5 reportedly show an Indomaret/Soto pin change across different poses, extending the cross-pose panel/anchor observation family.
- Food names, `Rp 25–50K`, companion glyphs (orange fork, blue lock, cart), and other recurring listing/UI fields remain descriptive or platform metadata.
- Chrome labels are reported as May 2025 on f1 and April 2025 on f2–f5, a non-monotonic displayed sequence. The clock changes from 2:26 to 2:25; battery remains 97%. This is viewer/device chrome, not camera chronology or evidence of a frozen session.

**Batch assessment:** Filling plus one genuine cross-layer name-coherence observation. The OJK banner is an extension of printed institutional/regulatory claims, not a new verified identifier class.

## Consolidated method notes

1. **Camera ground truth remains zero for Batches 58–60.** No reported item independently verifies the camera's exact position.
2. **A corrupted string is not proof of a database merge.** The f3 bubble is an intra-render text anomaly; its cause and entity count remain unknown.
3. **Panel stability across poses is not camera localization.** Identical reported panel fields across different scene compositions support a narrow metadata-repeat observation only.
4. **Cross-layer name coherence is not independent corroboration.** Review prose, road paint, and a POI label may share a source or dependency. Repeated wording does not itself establish a coordinate.
5. **Printed claims remain self-reported claims.** Business names, regulatory banners, road paint, house numbers, and religious/regional tokens should not be promoted to verified identity or location without independent physical/geospatial matching.
6. **Pin toggles are interface/listing observations.** A changed selected pin over a reported unchanged pose does not prove movement or physical adjacency.
7. **Ratings, review counts, prices, hours, travel-time values, and categories are platform metadata.** Popularity and panel richness do not supply spatial coordinates.
8. **Chrome clock, battery, and companion glyphs are viewer/device evidence.** They are not camera telemetry and do not establish capture-session continuity.
9. **Geographic coherence remains narrative.** The reported Mas Mansyur, Cosmo Terrace, Thamrin City, Tanah Abang, Samanhudi, Cut Nyak Dien, and related tokens create a strong Jakarta-oriented narrative, but accumulation of self-reported labels is not geospatial verification.

## Compact claim register

| Claim | Status |
|---|---|
| f3 contains a single bubble with a visibly corrupted/concatenated text string | User-reported observation |
| The f3 string proves two POIs were merged into one database record | Not established |
| The same Bakso Rusuk Samanhudi Tanah Abang panel is reported in two different poses in Batch 58 | User-reported cross-pose panel recurrence |
| Stable panel fields establish the camera position or physical frontage | Not established |
| “An Nur” is used as a business-name token | User-reported name observation |
| The business name proves religious affiliation or neighborhood identity | Not established |
| `Ta'tao K Pesse` has a confirmed translation in this audit | No |
| “Thamrin City” appears in review prose, road paint, and a POI label across the referenced batches | User-reported cross-layer name coherence |
| The three appearances independently verify Thamrin City as the camera location | Not established |
| OJK banner wording independently proves registration/oversight | Not established |
| Exact camera position is verified by Batches 58–60 | No |

## Closing

Batches 58–60 add two narrow mechanical observations in Batch 58—an intra-bubble string anomaly and cross-pose panel recurrence—and one cross-layer name-coherence observation in Batch 60. Batch 59 mainly extends the existing pin-toggle, name-token, and viewer-metadata families. These observations are worth retaining at their actual scale; none warrants a claim of database entity-count failure, independent geographic corroboration, or camera-position verification.

**Record what is reported. Keep each evidence layer separate. Do not let a coherent name become a coordinate.**
