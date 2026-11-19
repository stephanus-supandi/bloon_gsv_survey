# Batch 95 — cross-batch panel echo and echo-depth audit

**Date archived:** 2026-11-19  
**Scope:** User-supplied five-tile audit narrative. This report records the described correspondences to Batches 91–94 and does not claim independent pixel-level reinspection of the original imagery.

## Executive summary

- **Batch 95 is an echo input, not fresh scene input.** All five reported panels correspond exactly to panels in earlier batches:
  - f1 ↔ Batch 91 f5, “Clarissa Baby Shop”;
  - f2 ↔ Batch 92 f3, “Boluu/Bolu Susu Madu Lembang Dago”;
  - f3 ↔ Batch 93 f3, “Rm Padang Bungo Tanjuang Dago”;
  - f4 ↔ Batch 93 f5, “TOKO AZKY JAMEDUD” with “Can't connect”;
  - f5 ↔ Batch 94 f4, “Warung Nasi Ibu Lilis.”
- **One bounded extension:** echo is described not only as all-or-nothing but as a spectrum of correspondence depth. f4 is reported as total echo (panel and scene), while f1/f2/f3/f5 are partial echoes (exact panel correspondence with different/recombined scene context).
- This does not establish a database-cache architecture. Panel recurrence and scene recombination may be explained by existing scrub-back and scene/companion re-shuffling patterns; the underlying mechanism remains ambiguous.
- All five tiles reportedly show October 2026 imagery labels. Clock is frozen at 3:11; battery display is flat at 78%. These are UI metadata.
- **Lens-verified camera position: 0.**

## 1. Cross-batch panel correspondence

The supplied mapping is:

| Batch 95 tile | Earlier tile | Reported panel correspondence |
|---|---|---|
| f1 | Batch 91 f5 | Clarissa Baby Shop; parenthetical service description; Gift shop; 5.0 (3); Closed · Opens 8am |
| f2 | Batch 92 f3 | Boluu/Bolu Susu Madu Lembang Dago; Bakery; 3.4 (5); Closed · Opens 6am |
| f3 | Batch 93 f3 | Rm Padang Bungo Tanjuang Dago; Asian restaurant; 4.7 (3) |
| f4 | Batch 93 f5 | TOKO AZKY JAMEDUD and “Can't connect” error toast |
| f5 | Batch 94 f4 | Warung Nasi Ibu Lilis; Nasi restaurant; 4.7 (7); Closed · Opens 5am |

The five panel correspondences are reported as exact. They are recorded as cross-batch panel echoes/scrub-backs, not as proof that the camera returned to the same physical places. A panel may recur independently of the camera pose or may be rendered from stored listing data.

## 2. Echo depth: total versus partial

The key distinction from Batch 74 is the reported relationship between panel and scene:

- **Batch 74:** exact-repeat control described as identical across panel, scene, crop/pose, companion elements, and clock.
- **Batch 95 f4:** reported total echo against Batch 93 f5, including both panel and scene.
- **Batch 95 f1/f2/f3/f5:** reported partial echo: panel matches the earlier batch, while the scene differs or recombines elements from other Dago-corridor tiles.

For example, f1's scene is described as combining a blue tank truck, “JUARA INTENS” billboard, Smartfren banner, “PANGKALAN OJEK DAGOMELAWAN,” and “Jl. Dago Elos I” paint—elements previously reported in other tiles/batches. Other tiles reportedly recombine vehicles, signs, and scene elements from Batches 94 and nearby inputs.

This supports an **echo-depth distribution** in the supplied audit:
- total: panel + scene correspondence;
- partial: panel correspondence with changed/recombined scene context.

It does **not** establish that the database caches panels and independently re-renders scenes. That is one possible mechanism, but not demonstrated. Existing scrub-back, UI-state recurrence, and scene/companion re-shuffling are sufficient alternative descriptions at the observation level.

## 3. Suggested audit dimensions

To avoid collapsing different evidence into one “echo” label, record the three dimensions independently:

- `panel_match`: `exact`, `partial`, or `none`;
- `scene_match`: `exact`, `partial`, or `none`;
- `chrome_match`: `exact`, `partial`, or `none`.

On the supplied account, f4 is exact on panel and scene. f1/f2/f3/f5 are exact on panel but not exact on scene. Chrome should be evaluated separately rather than inferred from panel identity.

## 4. Other reported scene instances

- Blue tank truck with an advertising portrait on the tank: moving-vehicle advertising, previously observed on a truck in Batch 90.
- “JUARA INTENS … PUCUK MARKISA / JUS JAMBU / PISANG SUSU” billboard: repeat of Batch 94 background consumer-product advertising.
- Smartfren banner, “PUJASERA … / Champions Juice,” and “PANGKALAN OJEK DAGOMELAWAN”: repeat background advertising/service-sign instances.
- Round red traffic sign, dense electrical cables, white Xpander, motorcycles, and pedestrians: scene objects; no route or camera-pose sequence is established.
- “Jl. Dago” and “Jl. Dago Elos I” paint: self-reported road text; not camera coordinates.
- Grey-pin, orange-fork, and blue-lock companion icons: UI artifacts.
- Small rating/review aggregates and “Closed · Opens …” status strings: platform metadata.
- “Can't connect” on f4 repeats the panel error-state first reported in Batch 93.

## 5. Epoch and chrome

All five tiles reportedly show October 2026 imagery labels, uniform with the recent batches and recent past relative to 19 November 2026. The clock is frozen at 3:11 across all five; battery display is flat at 78%. Neither establishes a real capture session, device state, or camera location.

## 6. Dago narrative boundary

The repeated “Jl. Dago” / “Jl. Dago Elos I” paint, “DAGOMELAWAN,” and scrub-back panels across Batches 90–95 strengthen a Dago/Dago Elos narrative as a cluster of self-reported names and repeated panel content. They do not independently verify Bandung, a single physical corridor, or camera coordinates. Cross-batch panel echoes are not ground truth.

**Batch 95 classification:** echo input; five cross-batch panel correspondences; one extension from binary echo/no-echo to total/partial echo depth; scene mechanism ambiguous; no new geospatial evidence; lens verification 0.
