# BLOON GSV Candidate Field Notes — Jl. Nurtanio and Surrounding Streets

**Record date:** 2026-10-31  
**Repository:** `stephanus-supandi/bloon_gsv_survey`  
**Status:** `CANDIDATE / UNVERIFIED`  
**Evidence basis:** User-provided written descriptions of Google Maps Street View screenshots. The original screenshot files and panorama coordinates were not available in this upload operation.

## 1. Scope

The supplied descriptions cover a possible street network containing:

- Jl. Nurtanio
- Jl. Surya Dharma
- Jl. Melati VII
- Jl. Nakula 3
- Jl. Nakula 3A
- Jl. Bintang II
- Jl. Kakatua
- Jl. Cendrawasih

The descriptions suggest a mixed-use main street and quieter residential side streets. They do **not**, by themselves, establish that all listed streets belong to one neighborhood, one administrative area, or even one continuous road network.

A Bandung-area attribution was proposed in the supplied descriptions because of the name Jl. Nurtanio and the perceived proximity to Husein Sastranegara Airport. Treat that attribution as a **hypothesis only** until checked against coordinates and authoritative map/address evidence.

## 2. Candidate observations from the supplied descriptions

| Candidate location / label | Reported visible or map information | Classification | Verification status |
|---|---|---|---|
| 82 Jl. Nurtanio | Street marking reportedly reads “Jl. Nurtanio”; address label 82 | Street/address observation | Unverified; screenshot not independently inspected |
| Heri Cell | Mobile-phone counter; yellow banner; reported 5.0-star Maps rating | Business candidate | Unverified |
| Yanti Laundry | Laundry beside Heri Cell; reported opening time 08:00 | Business candidate | Unverified |
| Rumah Makan Padang Mutiara Minang | Restaurant name reportedly visible | Business candidate | Unverified |
| Mie Ayam Jamur / Ayam Penyet Nugraha | Food-stall sign reportedly visible | Business candidate | Unverified |
| Donna Donat | Maps label; reported 4.9 stars, 110 reviews, price range Rp25,000–50,000, opening 08:00 | Map-label/business candidate | Unverified; possible nearby/shared-frontage ambiguity |
| 29 Jl. Nurtanio / AYNARA | “AGEN RESMI ZOYA” banner reportedly visible | Business/signage candidate | Unverified |
| Nasi Kebuli Al-Wasllah 53 | Menu board reportedly lists egg, chicken, and beef variants | Business candidate | Unverified |
| Outlet Branded | Clothing-store sign/category reportedly shown | Business candidate | Unverified |
| Toko Sembako Rayyan | Grocery-store name reportedly visible | Business candidate | Unverified |
| Lucuna Car & Care | Automotive service sign/name reportedly visible | Business candidate | Unverified |
| Dapur Lucuna | Possible home-based food/catering operation | Business candidate | Inference; unverified |
| Kebab Turki “Lazis” | Kebab sign; Maps reportedly lists 16:00 opening | Business candidate | Unverified |
| Warung El Jago | Banner reportedly visible; possible proximity to Donna Donat | Business/signage candidate | Relationship to Donna Donat unverified |
| JKL Laundry & Dry Clean | Laundry sign; reported opening 08:00 | Business candidate | Unverified |
| Sate Madura Cak Hasan | Satay vendor name reportedly visible | Business candidate | Unverified |
| Distributor Beras Bulir Baik | Rice distributor name; Maps reportedly categorizes it as “Farm” | Business candidate | Category mismatch requires review |
| biMBA-AIUEO Jatisari Permai | Early-learning center label; reported 5.0-star rating | Business candidate | Unverified |
| Alfamart | Convenience-store label/sign reportedly visible | Business candidate | Unverified |
| 43 Jl. Nurtanio / Jl. Surya Dharma | Street intersection label; students and red hydrant reportedly visible | Street-scene observation | Unverified |
| Athaariq Corner 02 Surya Dharma | Grocery-store label; reported 5.0-star rating | Business candidate | Unverified |
| 20 Jl. Nakula 3 | Possible car-wash/service banner | Address/signage candidate | Unverified |
| 17 Jl. Nakula 3 | “DIJUAL” property banner; ERA / ERA SKY and contact name “NIA” reportedly visible | Property-sign observation | Unverified; personal phone number intentionally not transcribed |
| 59 Jl. Nakula 3A | Street View label reportedly says 59; house wall reportedly appears to show number 54 | Address conflict | Unresolved |
| 19 Jl. Nakula 3 | Two visually different properties reportedly carry the same Maps address label; one house plate reportedly reads “C20” | Address/panorama conflict | Unresolved |
| Jl. Bintang II | Street View imagery reportedly dated August 2022 | Street-scene candidate | Unverified |
| Jl. Kakatua | Street View imagery reportedly dated February 2021; food cart and playground described | Street-scene candidate | Unverified |
| Jl. Cendrawasih | Street View imagery reportedly dated March 2025; Toko Cendrawasih and park described | Street-scene candidate | Unverified |

## 3. Material inconsistencies and caution flags

### 3.1 Geographic attribution is not established

The supplied narrative proposes Bandung, and at different points mentions Cibuntu, Ciumbuleuit, Jatisari, and Jatisari Permai. These place names are not sufficient to prove a common location. Do not assign a city, district, village, or housing-estate identity to the whole set without coordinate-level checks.

### 3.2 Political-poster inference is weak

A poster reportedly mentioning “Mas Tri Adhianto” was used in the supplied narrative to support a Bandung attribution. A campaign poster is not a reliable geocoder by itself. The identity, campaign period, poster context, and actual panorama location must be independently verified before drawing a geographic conclusion.

### 3.3 Street View address labels may not match the visible property

Reported conflicts include:
- Maps label “59 Jl. Nakula 3A” versus a visible wall number that may read “54”.
- Repeated “19 Jl. Nakula 3” labels attached to different-looking properties, one reportedly bearing a “C20” plate.
- Possible adjacent or shared-frontage businesses around Donna Donat, Warung El Jago, and the Mie Ayam stall.

These are unresolved observations, not proof of incorrect mapping or duplicate addresses.

### 3.4 Street View dates are image metadata, not survey dates

The reported dates (February 2021, August 2022, and March 2025) must remain attached to their respective panoramas. Do not combine them into one contemporaneous snapshot of neighborhood conditions.

## 4. Required next verification steps

1. Recover the original screenshots or Street View share links for each observation.
2. Record panorama coordinates and imagery dates separately.
3. Verify street names and intersections using more than one independent map or address source.
4. Match each business pin to its exact frontage; do not infer adjacency from a bottom-sheet label alone.
5. Keep visible signage, Google Maps labels, and analyst inference in separate fields.
6. Resolve address conflicts only with direct visual evidence, coordinates, or authoritative address records.
7. Do not add these candidates to the verified master CSV until the location and evidence fields are complete.

## 5. Suggested data model

Use separate fields rather than a single “verified” label:

- `observed_text`: wording actually legible in the image
- `maps_label`: label shown by Google Maps
- `streetview_address_label`: address displayed by Street View
- `visible_property_number`: number physically visible on the building
- `business_category_claimed`: category shown by the map or sign
- `inference`: analyst interpretation, explicitly marked
- `panorama_date`: imagery date, if displayed
- `latitude`, `longitude`: exact panorama or POI coordinates
- `evidence_ref`: screenshot filename or Street View URL
- `verification_status`: `NOT_VERIFIED`, `PARTIAL`, or `VERIFIED`
- `conflict_note`: unresolved disagreement between evidence sources

## 6. Current conclusion

This is a useful **candidate field-note set** for further Street View archaeology. It is not yet a verified neighborhood inventory, geospatial dataset, or proof that all named streets and businesses belong to one Bandung-area residential complex.

**BLOON rule:** OBSERVED is not the same as MAP_LABEL. MAP_LABEL is not the same as VERIFIED. Proximity is not proof of adjacency. Unknown is not zero.

**GOBLOK BOLEH. NGARANG JANGAN.**
