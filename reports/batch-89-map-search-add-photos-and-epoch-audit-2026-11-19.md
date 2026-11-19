# Batch 89 — map search, contribution affordance, and imagery-epoch audit

**Date archived:** 2026-11-19  
**Scope:** User-supplied five-tile audit narrative: three map/search tiles and two Street View tiles. This report preserves the distinction between visible UI, imagery metadata, name/category fields, and geospatial evidence. It does not claim independent reinspection of the original imagery.

## Executive summary

- **Three configurations across two render media:** f1–f3 are map/search configurations; f4–f5 are Street View panoramas at different reported imagery epochs. This is not three distinct media types.
- **One UI-affordance extension:** “Add photos” is visible on f1/f3. It is a contribution affordance, not proof that an entity has no photos.
- **One epoch observation:** September 2026 is the newest imagery epoch reported in this corpus at this point and is about 18 months after March 2025. Relative to the actual date of this audit (November 2026), September 2026 is recent past, not a future calendar date.
- **One metadata anomaly candidate:** “God love his children” is rendered as “Housing complex · 21 min.” The name/category relationship is incongruent but ambiguous; no database-error claim is established.
- **Lens-verified camera position: 0.**

## 1. Render-medium and interface-state dimensions

The supplied description separates the five tiles as follows:

- f1–f3: map/search results, including the explicit query “children of god,” “See similar places,” and “Kacharavedu cricket ground.”
- f4: Street View imagery labelled March 2025.
- f5: Street View imagery labelled September 2026.

The accurate description is **three configurations across two render media**: map/search and Street View. The map/search tiles have no Street View imagery epoch chrome. The differing modes and epochs do not establish a single continuous capture sequence or camera route.

For future audit consistency, keep three fields independent:

1. `render_medium`: `street_view_panorama`, `map_2d`, or `unknown`.
2. `interface_state`: place panel, date selector, search result, contribution affordance, recently viewed, error state, or other visible UI.
3. `imagery_epoch`: visible imagery-date label, or missing/not applicable.

This prevents a map canvas, a search state, and an imagery-date label from being conflated as one “mode.”

## 2. “Add photos” contribution affordance

Tiles f1/f3 reportedly show “Add photos.” This extends the interface-state inventory beyond date-history and “Recently viewed” affordances.

The visible control is evidence only that the UI presents a contribution affordance. It does **not** establish that the corresponding entity has no photos, that the photo gallery is empty, or that a contribution backend was successfully invoked.

Suggested coding: `contribution_affordance_visible = true`; do not code `entity_photo_absence_confirmed`.

## 3. September 2026 imagery epoch

Tile f5 reportedly carries a September 2026 imagery label, while f4 carries March 2025. The September 2026 label is the newest reported epoch in this accumulated sequence and is roughly 18 months later than March 2025.

The actual audit date is 19 November 2026. Therefore September 2026 is not a future calendar date; it is recent past. It is a forward jump relative to the earlier corpus, not evidence of a future-rendering mechanism.

The epoch label remains imagery metadata. It does not provide camera coordinates or establish the date on which the screenshot itself was captured.

## 4. Name/category and radius ambiguity

The reported listing **“God love his children”** is paired with **“Housing complex · 21 min.”** Two broad interpretations remain possible: a residential complex with a religiously phrased name, or a name/category mismatch in the rendered listing. The tile alone cannot decide between them. “21 min” is travel-time/radius-style metadata, not a bearing or camera coordinate.

Other reported instances:
- Two variants of “Children of God's Kingdom” church naming: string variants, not automatically two entities or one verified entity.
- “Kacharavedu” / “Kaccharavedu”: spelling/string variation; identity unresolved.
- “Kacharavedu cricket ground”: sports-venue category inventory, not geospatial verification.
- User-photo strip reportedly showing people praying in front of a blue curtain and balloons: photo content only; it does not prove the event, date, or identity of participants.
- “Borneo Cuci Motor” rendered as “Car wash”: island/geographic token in a business name; not a location anchor.
- “138 A” on a pillar: visible number string, not a verified address without context.

India/Telugu/cricket references return to material already present in the earlier India-related corpus; they do not constitute a newly discovered continent or verified camera location.

## 5. Chrome and remaining limits

The Street View tiles reportedly show f4 at 5:01 and f5 at 3:15, with battery display increasing from 73% to 77%. These are UI readings, not evidence of physical device charging, capture-session chronology, or camera movement. Map/search tiles lack Street View epoch chrome.

**Batch 89 classification:** fresh input; extension of map/search configuration and contribution-affordance inventory; September 2026 is recent past relative to November 2026; metadata/name anomaly unresolved; no verified camera position.
