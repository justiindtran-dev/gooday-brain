# Marketing bot: ad pack sprint, 2:37 PM Sat 28 Nov 2026 (run-1437)

Files: `../../gooday-launch/static-ads/daily/2026-11-28/run-1437/` (finals, all versions, and `source/` with scripts, configs, masks and PHOTO-CREDITS.txt). Competitor reference crops (internal only): `../../gooday-launch/static-ads/daily/2026-11-28/refs/`.

Drafts only. Nothing was sent, posted, ordered or spent. The raw stand-in crops in `source/standin/` show another brand's pack and are **internal only**.

## What's new this run (variety, as asked)
Justin already has many similar table and hand shots, so neither design is a table or hand scene:
- **D1: clean studio pack shot on a solid flavour-colour field**, in the style of the approved "Zero shaker" and "Fibre, squeezed." ads. The pack is the realistic old spouted shape, volume ON. This is the first studio-field ad using the realistic pouch: before this, the approved field ads used the older glossy render.
- **D2: two-pack colour-block flat lay** (green grape fibre + peach collagen) on two sheets of coloured paper, teal and peach.
- **How the realism carries over without a table:**
  - Each pack's film cues (shading, long highlight streaks, seal-edge detail) come from one of Justin's **set-2 photos not used before**: 1000054849 for D1, 1000054851 and 1000054854 for D2.
  - Each pack's **soft shadow is fitted to the real shadow** that the stand-in casts in that same photo (photo / clean plate ratio, cast + contact model), then applied to our outline on the paper.
  - The two D2 packs come from two different photos, so their creases don't repeat. Both are at the same scale.
- **New pipeline keys** in `source/oldshape/oldshape.py`:
  - `base_full` composites onto a studio field, or onto an earlier pack render for a two-pack shot. The shadow is still fitted to the real photo.
  - `shadow_gain` adjusts the fitted shadow's density.
  - New scripts: `standin/field.py` (one-colour paper sweep with key-light falloff and paper tooth), `standin/field2.py` (two overlapping sheets, with a thin real-looking edge shadow), `standin/lfclean.py` (smooth clean plate used only to measure the shadow).

## Scores (finals)

| # | File | Headline | Scroll-stop | One message | Product visible | Thumbnail | Brand look | CTA | Believable | Looks real |
|---|---|---|---|---|---|---|---|---|---|---|
| D1 | `D1_B_FibreYouDontStir.png` (= v2) | Fibre you don't stir. | 4 | 5 | 5 | 4 | 5 | 4 | 5 | **4** |
| D2 | `D2_AB_OnesFibreOnesCollagen.png` (= v3) | One's fibre. One's collagen. | 4 | 4 | 5 | 4 | 5 | 4 | 5 | **4** |

**Why "looks real" is 4, not 5 (honest):**
- The pack outline and cap are drawn, and the dome and paper are modelled.
- The shadow model is fitted to a real shadow, but it is not photographed on that paper.
- D2's peach pack keeps two faint real film streaks on its maroon panel. They read as film glare, but they are visible at 100% zoom.
- A photo of a real printed Gooday mock-up on coloured paper is still the only route to a 5.

## D1 · B fibre (GREEN APPLE) · "Fibre you don't stir." (studio pack shot, solid leaf-green field)
- Copy:
  - Cream headline, 150 px.
  - Sub: "Green apple flavour. / 6 g fibre per pouch."
  - Cream pill "Join the waitlist".
  - Footer on a light scrim.
- Scene:
  - Leaf-green paper sweep (#336A31) with key-light falloff from the upper right. The real shadow falls toward the camera.
  - Green apple pack lying at a tilt, as in "Zero shaker", about 52% of frame height.

| Version | Scroll-stop | One msg | Product | Thumb | Brand | CTA | Believable | Looks real | Flaws |
|---|---|---|---|---|---|---|---|---|---|
| v1 | 4 | 5 | 5 | 4 | 5 | 4 | 5 | 3 | The shadow almost vanished on the dark field, so the pack looked stuck on. The field was flat and over-saturated with no light falloff. The "6 g" print rippled too much (crease displacement). The CTA sat close to the pack corner |
| **v2 (final)** | 4 | 5 | 5 | 4 | 5 | 4 | 5 | 4 | Lighter field with stronger falloff. Fitted real shadow density ×1.35 (cast) / ×1.2 (contact). Ripple halved (disp 2). Grey smudge on the white panel lifted (`s_floor`). Sub moved under the headline. Remaining: faint green bounce on the pack edge, a little too even |
| v3 (rejected) | 4 | 5 | 5 | 3 | 5 | 3 | 5 | 4 | Tighter crop for a bigger pack, but the CTA then covered the pack's bottom corner. Kept v2 |

## D2 · AB both lines · "One's fibre. One's collagen." (two-pack flat lay on teal + peach paper)
- Copy:
  - Cream headline on the teal sheet.
  - Maroon sub on the peach sheet: "Green grape: / 6 g fibre per pouch. / Peach: / 5 g collagen per pouch."
  - Maroon pill "Join the waitlist".
  - Footer on a light scrim.
  - No kcal line (kcal is only for the fibre pouch, and the collagen pouch is also in frame).
- Scene:
  - The peach pack lies on the teal sheet and the grape pack on the peach sheet, each colour-blocked against the other.
  - The peach sheet lies over the teal, with a thin edge shadow.

| Version | Scroll-stop | One msg | Product | Thumb | Brand | CTA | Believable | Looks real | Flaws |
|---|---|---|---|---|---|---|---|---|---|
| v1 | 4 | 4 | 5 | 3 | 5 | 4 | 4 | 3 | The peach pack rendered about 7% smaller than the grape pack (same real size, so it reads fake). The sub copy sat on top of the grape pack and couldn't be read. The grape pack straddled the colour split, teal on teal. The peach paper had blotchy mottling |
| v2 | 4 | 4 | 5 | 3 | 5 | 4 | 5 | 4 | Packs at equal scale, separated, each on its contrasting sheet. Split re-angled. Mottling cut. Remaining: the sub straddled the split (maroon on teal can't be read), and drawn streak lines on the peach pack's maroon panel looked like scratches |
| **v3 (final)** | 4 | 4 | 5 | 4 | 5 | 4 | 5 | 4 | Sub moved to the clear peach area (right, 4 short lines). Drawn streaks removed or softened (kspec 0.5). Remaining: two faint real film streaks on the maroon panel; empty lower-left corner |

## Gooday design | competitor reference + stats | what we borrowed and changed
Source: **Justin's real TrendTrack screenshots** (`style-references/trendtrack-swipes-2026-11-27/`, captured 27 Nov). Stats are read off the screenshots. Nothing is estimated. Neither ad was used earlier today; the crops are new.

Ad IDs are not visible in the screenshots, so there are no direct ad links. To find them, use TrendTrack → goli.com → Ad Library, or the [Meta Ad Library search for Goli](https://www.facebook.com/ads/library/?active_status=active&ad_type=all&country=US&q=goli).

**Honest note:** both are short runs (9 days at capture), so they are not yet proven by run length.

| Gooday design | Competitor reference + stats | What we borrowed and changed |
|---|---|---|
| D1 "Fibre you don't stir." `run-1437/D1_B_FibreYouDontStir.png` | **Goli, Beauty Stik, "Hyaluronic acid meets jelly."**: bold two-line statement headline over one stick on a solid pink field with real strawberries, Meta. Crop `refs/goli-beautystik-hyaluronic-swipe10.png`. TrendTrack (swipe-10, card 2): **active 9 days (18 Nov → now)**, rank **114/269 (43%)**, trending up, no targeting data, variation count not shown. Why it works: a big format statement plus one pack on a field in its own colour reads in a second. | **Borrowed:** a bold statement headline on a solid field in the pack's colour, with one tilted pack as the hero. **Changed:** our statement is a format fact (no stirring, Green "no mixing"), not an ingredient or benefit claim. No skin, hair or "supports" lines, no coupon codes or discount, no "made in" line, no jelly ooze shown (ACCC 128/26). Real fitted shadow on paper instead of a glossy render. None of their words, pack or branding. |
| D2 "One's fibre. One's collagen." `run-1437/D2_AB_OnesFibreOnesCollagen.png` | **Goli, "3 delicious jelly STIKS"**: the whole range together (3 boxes on a shelf + sticks in a basket), Meta. Crop `refs/goli-stiks-trio-shelf-swipe07.png`. TrendTrack (swipe-07, card 1): **active 9 days (18 Nov → now)**, rank **11/269 (5%)** (best rank in the swipes), trending up, targeting US +94 countries (more locked behind Pro), **2 variations**. Why it works: showing the range at once says "pick yours" without words. The caption leans on a bundle and "FREE" offer. | **Borrowed:** the range shown together in one frame, one pack per flavour/line. **Changed:** two pouches on colour-blocked paper, not a styled bathroom shelf. Each pack is named with its Green claim only (6 g fibre / 5 g collagen per pouch). No bundle, no "free", no offer, no benefit icons (their range sells sleep, gut and beauty benefits; we show none), no "new format" hype. |

## Compliance self-check (against brain/claims.md, incl. Rules learned 27 and 28 Nov)

| Item | Line | Ruling |
|---|---|---|
| D1 headline | "Fibre you don't stir." | PASS. A format fact (Green: "no mixing, no shaker"). No health, gut, dose or result claim, nothing about the viewer's body, no competitor named or compared |
| D1 sub | "Green apple flavour. 6 g fibre per pouch." | PASS. "6 g fibre per pouch" is Green. No kcal line on the apple pack (28 Nov kcal rule kept conservative) |
| D2 headline | "One's fibre. One's collagen." | PASS. Describes the two products. No ranking, no "take both daily" dose language |
| D2 sub | "Green grape: 6 g fibre per pouch. Peach: 5 g collagen per pouch." | PASS. Both Green. No kcal (the collagen pouch has no kcal line until tested). No skin, hair, joint or recovery claim |
| Pack print (both) | `_k` flats: "6 g fibre per pouch" / "5 g collagen per pouch", "Fibre + greens jelly" / "Collagen jelly", flavour, "Squeeze & go / No scoop, no shaker, no mixing" | PASS. "Good source of fibre" and "Marine collagen peptides" erased. The greens/sugar and Kakadu lines are soft-focused (unreadable). No "TEAR HERE" on a screw-cap pack. Net/kJ erased |
| CTAs | "Join the waitlist" | PASS. No urgency, timer, discount or "be first" |
| Footers | "Not on sale yet. Concept pack shown. Nutrition figures are targets and will be confirmed before launch." | PASS. Readable on a phone: white on a light dark scrim over a plain field (27 Nov rule). The finals show only our old spouted shape, never the stand-in silhouette, so "Concept pack shown" is the right footer (28 Nov rule) |
| Images (ACCC 128/26) | Rendered packs with fitted real shadows on a modelled paper field | PASS for waitlist use with the footer. Normal fill, no jelly, gloss or texture not photographed. Both packs at the same true scale. Before pre-orders, sales or any price, swap in photos of the real or printed pre-production pack |
| Competitor rules | | PASS. No competitor named, no logos, characters or wording copied, no fake urgency or discounts |

**Result: PASS (both finals).**

## Method notes (reusable; scripts in `run-1437/source/`)
1. **Studio field with real-photo realism:**
   - Pad the stand-in photo and its clean plate so the pack can sit anywhere in the frame.
   - Render with `base_full` = the field. The shadow model is fitted to the stand-in's real shadow, so softness, offset and density come from the photo.
   - On a dark field, raise `shadow_gain` (about 1.3) or the shadow disappears.
   - `bounce` then picks up the field colour on the pack edges (correct for coloured paper).
2. **Strongly tilted, foreshortened stand-in** (photo 49): auto tilt failed (it read 6°), so set `rot_deg` by hand (-22).
3. **Two-pack:**
   - Render the back pack onto the field first, then the front pack with `base_full` = that render, so its shadow falls on the first.
   - Use packs from different photos of the same session, so the creases don't repeat.
   - Match `scale_k` so both packs come out the same size.
4. **Drawn streak paths** (`*_streaks.json`) look like scratches on dark panels (maroon). Keep them faint (i 0.3) or leave them out there.
5. **Mount lag:** files written by one script can take a few seconds to appear to the next. Wait before chaining.

## Question for Justin
Approve D1, D2, both, or neither? Approved designs go to `static-ads/approved/2026-11-28/` and the Miro "Approved ads" frame.
