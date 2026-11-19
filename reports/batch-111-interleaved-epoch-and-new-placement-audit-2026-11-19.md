# Batch 111 — Interleaved epoch and new-placement audit

**Date:** 2026-11-19  
**Scope:** Five user-supplied Street View tiles in the Kelapa Gading / Gading Kirana and Bukit Gading narrative corridor.

## Executive assessment

Fresh input; no new mechanical layer. Batch 111 refines the epoch-distribution inventory with an interleaved pattern and adds three thin extensions in where information appears: Hangul in a database-rendered name field, property-sale wording on printed media, and a foot pictogram on facade glass. **Lens-verified camera position: zero.**

## 1. Epoch pattern: interleaved, not contiguous

Batch 110 displayed [May 2025, July 2024, July 2024, July 2024, July 2024]. Batch 111 displays:

| Tile | Displayed epoch |
|---|---|
| f1 | July 2024 |
| f2 | May 2025 |
| f3 | May 2025 |
| f4 | July 2024 |
| f5 | July 2024 |

This is [July, May, May, July, July], an interleaved two-epoch pattern rather than a single contiguous block. It is a third observed distribution shape after the single-stale-frame and contiguous-block cases.

The pattern does **not** establish a database timeline, a systematic epoch block, or a particular navigation mechanism. It is compatible with manual navigation among previously available imagery, but the pixels alone do not prove that the user manually scrubbed cached frames. Cache reuse, source selection, navigation, and other serving/rendering explanations remain **AMBIGUOUS**.

The controlling principle from Batch 106 remains: an imagery epoch header is render metadata, not independent proof of when a frame was captured or of camera position. Batch 111 deepens the inventory of displayed epoch arrangements; it does not reverse the earlier demotion.

## 2. Clock and epoch: a metadata mismatch, not a session proof

Readable clock values include f2 (May 2025) at 8:51 and f4/f5 (July 2024) at 8:50. Thus tiles carrying different displayed imagery epochs carry adjacent, monotonically decreasing clock values.

This supports a narrow conclusion: **the displayed clock is not a reliable validator of imagery epoch**. It does not prove that every tile was rendered in one live session, that a live clock was advancing, or that the user manually switched between cached eras. A screenshot replay can preserve chrome embedded in the image; a live rendering could also, in principle, show repeated values. The precise mechanism is unresolved.

The f1 and f3 clock areas are cropped/unreadable. Battery display is 90% and remains a render-level value, not verified device state.

## 3. Three thin extensions in placement

- **Hangul in the database-rendered name field:** f5 displays “Masaji Family Massage 마사지”. Earlier non-Latin examples were visible in scene/facade or map-mode content; this is an instance in the rendered entity-name field. Whether the Hangul is owner-submitted branding or another presentation-layer contribution is **AMBIGUOUS**. It extends existing name-composition and non-Latin-token inventories; no new mechanical layer or geospatial anchor follows.
- **Property-sale printed media:** f4 shows “DIJUAL” banners with names and phone-number strings. This adds property-sale advertising as a semantic class within the printed-media inventory. The banners establish only that the wording is visible; property availability, ownership, seller identity, and transaction status are not independently verified. “Hub HERE” remains unresolved.
- **Foot pictogram on facade glass:** f2 shows a two-foot pictogram decal associated visually with an “Energy Massage” frontage. This extends facade-signage observations from text/logo to a service pictogram on glass. It is distinct from database companion glyphs. The decal is not a camera-position anchor.

## 4. Other observations and recurrences

- f1 “Notaris & PPAT Pauline Nataadmadja .SH” combines two professional designations in the rendered name field, an ampersand, and a leading-dot credential string. The personal name and credential interpretation are not independently verified.
- f2 and f5 both carry the “Massage therapist” category, with different displayed ratings, status strings, and accessibility metadata. This is within-batch densification of the wellness/service inventory, not a new category mechanism or proof of two verified operating businesses.
- f3 includes a “PAKET RAMADHAN … GRATIS …” promotion on a workshop facade. This extends printed-media examples to a seasonal religious token attached to a non-food service promotion; the banner alone does not establish campaign timing or business activity.
- f4/f5 show “Jl. Raya Bukit Gading” and “Villa” wording, with “Bukit Gading Indah” as a rendered name. This adds a residential/villa sub-enclave to the corridor's displayed toponymic narrative, alongside Gading Kirana. It does not verify a street grid, neighborhood boundary, or city.
- Other recurring elements include facade text/logo combinations, a BTS-style lattice tower, terminally truncated panel titles, ratings, companion glyph clusters, motorcycles, cars, people, cones, landscaping, and sparse panels. They remain scene or UI observations, not spatial anchors.

## 5. Corridor narrative and limits

The displayed strings lean toward Kelapa Gading / Gading Kirana / Bukit Gading / Jakarta as a **self-reported narrative**. The repeated toponyms and named sub-enclave enrich that narrative but do not establish ground location. No camera route, camera pose, city, or coordinate is inferred.

**Conclusion:** Batch 111 is a fresh, no-new-mechanical-layer batch. It adds an interleaved epoch arrangement and three placement extensions, while reinforcing the limited conclusion that displayed clock values cannot validate imagery epochs. The exact serving/navigation mechanism remains ambiguous. **Lens-verified camera position: zero.**
