# Batch 112 — Stale-at-end epoch and three-pin facade audit

**Date:** 2026-11-19  
**Scope:** Five user-supplied Street View tiles in the Bukit Gading / Kelapa Gading narrative corridor.

## Executive assessment

Fresh input; no new mechanical layer. Batch 112 adds a stale-at-end epoch arrangement and extends the multi-pin/same-facade inventory to three rendered pins spanning religious, travel, and security categories. It also adds a cross-shaped companion glyph instance and several naming/signage recurrences. **Lens-verified camera position: zero.**

## 1. Epoch pattern: stale frame at the end of a newer primary group

Per-tile displayed imagery epochs:

| Tile | Visible listing / scene lead | Displayed imagery epoch |
|---|---|---|
| f1 | Aditya Octavo Lumenco. PT | July 2024 |
| f2 | GBI Bethel Kelapa Gading | July 2024 |
| f3 | Sagas Security | July 2024 |
| f4 | Enka Tour | July 2024 |
| f5 | Agen Pos Shada Inc | March 2020 |

The sequence is [July, July, July, July, March]: a March 2020 tile at the end of a four-tile July 2024 group. This is a positional variant of the epoch-puncture inventory, distinct from the single-stale-frame case, Batch 110's contiguous multi-tile split, and Batch 111's interleaved pattern.

The stale tile's position at the end does not change the status of the epoch header: it remains displayed imagery metadata, not proof of capture chronology or camera position. Whether the old frame was served from cache, selected through imagery navigation, or supplied by another mechanism is **AMBIGUOUS**. The arrangement is recorded as a distributional observation, not a new database mechanism.

## 2. Clock/epoch relationship

Readable clock values are 8:50 on f1–f4 and 8:49 on f5. The March 2020 tile therefore carries a displayed clock one minute earlier than its July 2024 neighbor.

This repeats the narrow Batch 111 conclusion: **displayed clock values do not validate imagery epochs**. It does not prove that all frames were shown in one live session, that the clock was live, or that a particular manual scrub/cache mechanism occurred. Chrome may be embedded in a replayed image; the exact source of the displayed values is unresolved. Battery display remains 90%, a render-level observation rather than verified device state.

## 3. Three rendered pins associated with one apparent facade

Tiles f2, f3, and f4 show the same apparent yellow/glass building frontage across different poses. Two prominent signs recur in the background:
- “Pdt. Dr. RUBIN ADI ABRAHAM SUNDAY SERVICE 08:00 & 10:00”, also represented by the rendered pin “GBI Bethel Kelapa Gading” (Pentecostal church).
- “NARENDRA INVESTAMA CORPORATE GROUP / TRAVEL CONSULTANT / JL. Bukit Gading Raya Blok G No.7 / Kelapa Gading, Jakarta Utara 14250” with email and telephone details, also associated with the “Enka Tour” pin.

A third rendered pin, “Sagas Security” (Security system supplier), appears in the same apparent facade context. The three pins therefore span religious, travel, and security categories in one displayed imagery epoch.

This extends the multi-pin/multi-function facade inventory from two pins to three pins and three distinct rendered categories. It remains **AMBIGUOUS** whether these are actual tenants in one building, neighboring premises represented in the same view, a pin-placement mismatch, legacy names/listings, or another relationship. The sign and pin correspondence is visual association, not legal occupancy, ownership, exact co-location, or proof of database error. No coordinate or camera position is derived from the facade.

This differs from Batch 110's two-pin automotive/corporate facade case by the number and category spread of the rendered pins, not by establishing a new mechanism.

## 4. Other bounded observations and recurrences

- **GBI Bethel Kelapa Gading:** the rendered category is “Pentecostal church”. “GBI” is retained as an acronym string; no expansion is asserted from the frame alone. The pastor's name/title and Sunday service times appear on a facade sign, an instance of religious printed media and schedule wording, not independent confirmation of the service schedule.
- **Enka Tour:** the facade sign contains a corporate-group name, travel-consultant wording, a structured street address, email, and telephone number. These are visible self-reported sign contents, not independently verified contact details, address, operation, or ownership. “Jakarta Utara” is a printed location string, not camera ground.
- **Sagas Security:** rendered category “Security system supplier”, displayed rating 5.0 (5), and “Open · Closes 7pm” are platform metadata only. The rating is not a location measure; operating status is not independently verified.
- **Aditya Octavo Lumenco. PT:** the period before the legal-form suffix is a name-delimiter instance. “Computer support and services” is a rendered category; the name/identity is unresolved.
- **Agen Pos Shada Inc:** “Inc” is recorded as an English corporate-suffix instance alongside a postal-agent listing. The name remains unresolved. A foreground pickup truck partly occludes the scene; this is transient scene content.
- **Cross-shaped companion glyph:** a cross-like symbol appears among companion icons in the Enka Tour/Sagas Security panels. It extends the companion-artifact inventory; it is a UI-rendered glyph, not proof of religious affiliation, entity identity, or spatial position.
- Recurrent elements include the Bukit Gading / Villa toponymic strings, BTS-style lattice tower, orange cones, motorcycles, SUVs, people, palm trees, facade signage, sparse panels, terminal title truncation, ratings, and status metadata. They are retained as scene/UI recurrences.

## 5. Corridor narrative and limits

Visible strings strongly lean toward Bukit Gading / Kelapa Gading / Jakarta Utara as a **self-reported narrative**, including the printed address and repeated facade signage. Those strings do not independently verify the city, neighborhood boundary, exact address, or camera location. The three-pin facade observation does not convert signage into ground truth.

**Conclusion:** Batch 112 is fresh input with no new mechanical layer: one stale-at-end epoch arrangement, one three-pin/three-category same-apparent-facade observation, and a cross-shaped companion-glyph instance. Epoch, clock, battery, names, signs, categories, ratings, and companion icons remain render/display evidence. **Lens-verified camera position: zero.**
