# Jatiwaringin / Pangkalan Jati — incremental POI intake (2026-11-24)

## Record status

- **Status:** provisional intake from user-supplied summaries of Street View / listing screenshots.
- **Evidence basis:** textual descriptions supplied in chat; original screenshots, listing URLs, and Street View URLs were not independently inspected in this update.
- **Reported imagery labels:** February 2025 and April 2025, as supplied. No unsupported frame-to-POI mapping is inferred.
- **Geographic scope:** Jatiwaringin / Pangkalan Jati area, Bekasi, West Java, Indonesia. Road-area references are not exact addresses or coordinates.
- **Verification:** NOT VERIFIED. Names, categories, ratings, review counts, opening-hours claims, and location descriptions remain user-reported.
- **Coordinates / stable IDs:** none supplied; intentionally not assigned.
- **Current operating status / occupancy:** unknown.

## Intake D — Jatiwaringin / Pangkalan Jati (5 provisional POI candidates)

| Name as supplied | Provisional category | User-reported metadata / note |
|---|---|---|
| Arjuna Motor (Dealer Mobil Bekas) | Used-car dealer | 4.5★ (188 reviews). User clarifies this is the specific business inside the building previously labelled “Griya Soenjoto”. This is a new identity lead for the business within/at the scene; it does not establish that “GRIYA SOENJOTO” and “Arjuna Motor” are the same entity. |
| Pasundan Motor | Used-car dealer | 5.0★ (8 reviews) |
| Marugame Udon Jatiwaringin | Japanese restaurant / chain outlet | 4.6★ (3,647 reviews); reported at Jl. Pangkalan Jati IV |
| Warkop Babeh Royan | Cafe / warung | 5.0★ (1 review) |
| Evolution AutoSound | Car audio / stereo store | 4.9★ (16 reviews) |

## Intake E — Jl. Raya Jatiwaringin (5 provisional POI candidates)

| Name as supplied | Provisional category | User-reported metadata / note |
|---|---|---|
| PANDU FILM | Automotive / residential window-film specialist | Service scope reported; not independently checked |
| Mega Baja Jatiwaringin | Steel and building-materials supplier | No additional metadata supplied |
| Siomay Bandung Batagor | Street-food stall | Reported near STIE Swadaya; generic name, exact vendor identity unresolved |
| Subur Jaya Printing | Printing shop | 4.2★ (42 reviews); reported open 24 hours, not independently checked |
| Toko Hafif Zulfitrah | Grocery store | Reported next to Subur Jaya Printing; adjacency is user-reported and does not by itself establish a shared parcel or exact storefront boundary |

## Intake F — Jl. Raya Jatiwaringin / Kalimalang area (5 provisional POI candidates)

| Name as supplied | Provisional category | User-reported metadata / note |
|---|---|---|
| WARKOP PANCONG CERIA | Coffee shop / warung | Reported near Jl. S. Kalimalang |
| Lion Parcel - Maloho Parcel | Parcel / shipping service | 3.3★ (32 reviews) |
| OKI LAUNDRY kiloan, satuan, dry clean | Laundry service | 3.8★ (15 reviews) |
| Progress Foto Copy & Percetakan | Photocopy / printing shop | 4.3★ (7 reviews) |
| Mie Uleg Sedjuk | Noodle cafe / restaurant | 4.9★ (125 reviews) |

## Reconciliation with prior Jatiwaringin intake

The earlier field note dated 2026-11-24 records 13 provisional candidates, including GRIYA SOENJOTO and Auto Kreasi, plus the Shintasila Battery wider-frame repeat and Auto Kreasi's February/April re-observation.

New user-supplied clarification:
- **Arjuna Motor** is identified by the user as the specific used-car business inside the building previously labelled “Griya Soenjoto”.
- Preserve both strings as separate evidence fields: “GRIYA SOENJOTO” (earlier housing-complex listing/pin label) and “Arjuna Motor (Dealer Mobil Bekas)” (new business identity lead).
- Do not merge the two into one POI or conclude that the building, parcel, housing-complex label, and business are identical. A physical-site / POI relationship remains to be verified from original frames, pin positions, signage, and coordinates.

No other candidate in Intakes D–F is automatically merged with a prior POI based on generic category, name similarity, or proximity descriptions. A repository text search for the distinctive names supplied in this batch did not return existing matching records; this is a limited text-search duplicate check, not proof that no duplicate exists elsewhere in the full dataset.

## Intake accounting and running estimates

- Previous Jatiwaringin note: 13 provisional POI candidates.
- Intake D: 5 additional candidates.
- Intake E: 5 additional candidates.
- Intake F: 5 additional candidates.
- **Cumulative candidate count across these two field notes: 28 provisional POI candidates**, before any future image/coordinate-level deduplication.
- Earlier duplicate/re-observation controls remain: Shintasila Battery wider frame = same candidate; Auto Kreasi February/April = one candidate with two reported observation dates.
- New user-reported running estimates: Indonesia ~35; global total ~188 (Patchogue ~65, Mexicali ~65, New Delhi ~23, Indonesia ~35). These are observer estimates, not independently audited unique-POI counts. The arithmetic sum of the rounded regional estimates is approximately 188; rounding and unverified duplicate resolution remain.

## Method and exclusions

1. Preserve supplied names and metadata verbatim where practical; do not infer official legal names or normalize ambiguous strings without evidence.
2. Ratings, review counts, categories, opening-hours claims, and platform labels are metadata, not independent proof of identity, quality, occupancy, or current operation.
3. A pin on or near a building does not establish the business's premises, parcel, tenancy, or ownership.
4. A nearby-location description (for example, “next to”, “near STIE Swadaya”, or “near Kalimalang”) is contextual, not a coordinate.
5. No coordinates, stable IDs, legal ownership, exact addresses, current operating status, or parcel relationships are inferred.
6. This intake remains a separate field note. No normalized site–POI–observation records or master CSV rows are created pending source-image review and location-level verification.

## Evidence needed for the next verification pass

- Original screenshots or Street View share URLs for each candidate.
- Directly visible image date for each observation.
- Pin context and visible signage sufficient to distinguish a business from the building/site label.
- Coordinates only from a directly captured or independently verified map point.
- Cross-check storefront and pin positions before resolving the GRIYA SOENJOTO / Arjuna Motor relationship or any adjacent-business claim.
