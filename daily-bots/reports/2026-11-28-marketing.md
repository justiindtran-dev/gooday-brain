# Marketing bot: ad pack sprint, 4:58 AM Sat 28 Nov 2026 (run-0458)

Files: `../../gooday-launch/static-ads/daily/2026-11-28/run-0458/` (finals, all versions, `source/` with scripts, configs, masks, clean plates and PHOTO-CREDITS.txt). Competitor reference crops (internal only): `../../gooday-launch/static-ads/daily/2026-11-28/refs/`.

Drafts only. Nothing was sent, posted, ordered or spent. The raw stand-in crops in `source/standin/` show another brand's pack and are **internal only**.

## What's new this run
- **3 new scenes from Justin's own set-2 photos**, none used before: 1000054841 (open palm), 1000054850 (wood table, real apple removed), 1000054855 (top-down, his hand + his real apple). No stock images, no pasted fruit.
- **Old spouted shape, volume default ON** (filled-pouch dome, rim valley, core highlight, bowed sides, edge thickness, AO) via `source/oldshape/oldshape.py`, with only the stand-in photo's film cues (shading, highlight streaks, seal-edge detail, light colour) moved onto it.
- **Pack print updated for the coordinator's 28 Nov compliance notes** (new `_k` flats, `source/real/fixflat.py`):
  - "TEAR HERE" and the neck notches removed (the old shape has a screw cap).
  - The readable line is now "Squeeze & go / No scoop, no shaker, no mixing".
  - The Net 120 g / kJ row is erased, not just blurred.
  - Amber/open lines stay erased. The "plus greens / with Kakadu plum · under 2 g sugar" line stays soft-focused and unreadable.
- **New clean-plate tools:**
  - `rowfill.py` fills each row only from the same row, so the grain and depth blur match in a perspective photo, and it stops before a board joint.
  - `shiftfill.py` copies texture from a nearby clean patch (used for skin).
  - `applefix.py` rebuilds a fruit edge that the stand-in covered.
- **Original brand:** 100% removed. I zoom-checked all 3 for foreign text, the "0" mark, the tab and green film; none remains. Front views only.

## Scores (finals)

| # | File | Headline | Scroll-stop | One message | Product visible | Thumbnail | Brand look | CTA | Believable | Looks real |
|---|---|---|---|---|---|---|---|---|---|---|
| D1 | `D1_B_HeresYourFibre.png` (= v4) | Here's your fibre. | 4 | 5 | 5 | 4 | 4 | 4 | 5 | **4** |
| D2 | `D2_A_SoSorry.png` (= v2) | We're so sorry. | 5 | 4 | 4 | 4 | 4 | 4 | 5 | **4** |
| D3 | `D3_B_CrunchNow.png` (= v2) | Crunch now. Squeeze later. | 4 | 5 | 4 | 4 | 4 | 4 | 5 | **4** |

**Why "looks real" is 4, not 5 (honest):** the scenes, hands, apple, light and shadows are real photos, but zooming in still shows edits.
- The pack outline and cap are drawn, and the dome is modelled.
- D1 has a small softened skin patch left of the neck and a faint seam along the right body edge, where the fingers were rebuilt.
- D2 has a few crinkle specks on the film near the lower right seal.
- D3 has a faint dent on the apple's lower edge next to the cap, where the apple edge was rebuilt.

A photo of a real printed Gooday mock-up is still the only route to a 5.

## D1 · B fibre · "Here's your fibre." (green apple pack in Justin's open palm)
- Copy:
  - Cream headline on a dark top shade.
  - Dark-green **stat strip** on the right (stacked): "6 g fibre | no mixing | no shaker" (v4; v3 had "about 25 kcal", see the FIX below).
  - Cream pill "Join the waitlist". Footer on a dark scrim.
- Scene: photo 41 rotated 90° so the hand offers the pack upright. Pack about 70% of frame height, the biggest of any design so far.

| Version | Scroll-stop | One msg | Product | Thumb | Brand | CTA | Believable | Looks real | Flaws |
|---|---|---|---|---|---|---|---|---|---|
| v1 "Fibre, pouched." | 4 | 4 | 5 | 4 | 4 | 4 | 5 | 3 | Cream headline over the light thumb was hard to read; the stat column overlapped the pack edge; a pale smear of rebuilt skin showed left of the neck (the gap between thumb and palm) |
| v2 | 4 | 4 | 5 | 4 | 4 | 4 | 5 | 4 | Pack tilted 3.5° and moved 30 px left so its shoulder covers the smear; finger strip on the right rebuilt row by row (finger gaps continue); dark top shade; narrower strip clear of the pack. Remaining: "Fibre, pouched." repeats the "Fibre, X." headline pattern already used (25 and 27 Nov) |
| v3 | 4 | 5 | 5 | 4 | 4 | 4 | 5 | 4 | New headline that fits the open-palm "offering" scene. Remaining: faint seam on the right body edge; the strip is stacked vertically rather than a single row (no room under the pack) |
| **v4 (final)** | 4 | 5 | 5 | 4 | 4 | 4 | 5 | 4 | **Compliance FIX (coordinator, 28 Nov):** "about 25 kcal" is confirmed for the green grape fibre pouch only, and neither claims.md nor product.md gives green apple ~25 kcal. The middle row is now Green "no mixing". Everything else is unchanged from v3 |

## D2 · A collagen · "We're so sorry." (peach collagen pack on the wood table)
- Copy:
  - Maroon headline.
  - Body: "5 g collagen in a squeezable pouch. Peach flavour. No shaker. **It's still in development, so you can't buy it yet.**"
  - Maroon pill "Join the waitlist". Footer on a dark scrim.
  - No kcal line (28 Nov rule: collagen has no kcal line until it is tested).
- Scene: photo 50, with **his real apple removed** (D2 is peach). The wood was rebuilt row by row from the same photo, so the grain and blur match the depth. The pack lies where the stand-in lay, with the photo's own shadow model.
- Pack size about 44% of frame height. The empty wood above holds the apology copy.

| Version | Scroll-stop | One msg | Product | Thumb | Brand | CTA | Believable | Looks real | Flaws |
|---|---|---|---|---|---|---|---|---|---|
| v1 | 5 | 4 | 4 | 4 | 4 | 4 | 5 | 4 | White crinkle and scratch specks on the film at the lower right and left seal read as dirt; the body said "It's… It's…"; the key line (not on sale yet) didn't stand out |
| **v2 (final)** | 5 | 4 | 4 | 4 | 4 | 4 | 5 | 4 | Highlight streaks lowered (kspec 0.55, edge detail 0.3); body tightened, with the honest "can't buy it yet" line in bold. Remaining: the pack's dark lower half sits near the dark scrim; the body copy is 3 lines (more text than our usual style, by design for this hook) |

## D3 · B fibre · "Crunch now. Squeeze later." (green apple pack beside Justin's real apple, his real hand)
- Copy:
  - Green headline.
  - Subline "Green apple flavour. 6 g fibre per pouch." (top right).
  - Green pill "Join the waitlist" to the right of the apple. Footer on a dark scrim.
- Scene: photo 55, top-down, rotated so the cap points at the apple.
  - His real hand stays **in front** of the pack (thumb over the edge, holding it).
  - The stand-in's tab had covered the apple's lower edge. I rebuilt that edge from the apple's own skin, and the cap now sits against it.
- The real red/yellow apple is used honestly, with "Green apple flavour" (not colour-graded).

| Version | Scroll-stop | One msg | Product | Thumb | Brand | CTA | Believable | Looks real | Flaws |
|---|---|---|---|---|---|---|---|---|---|
| placement tests | – | – | – | – | – | – | – | 3 | Dropped before layout: 1) pack too low, with a bite-shaped gap in the apple; 2) pack too far left, with his thumb covering "6 g"; 3) pack too far right, so the hand no longer held it. Fixed by applefix.py + dx −25 / dy +50 |
| v1 | 4 | 5 | 3 | 4 | 4 | 3 | 5 | 4 | Pack only about 38% of height, with the apple competing; the CTA overlapped the pack's right edge; empty lower third of wood and joint |
| **v2 (final)** | 4 | 5 | 4 | 4 | 4 | 4 | 5 | 4 | Tighter crop (pack about 40%, apple and pack fill the middle); headline set smaller to fit above the apple; compact CTA moved beside the apple, clear of the pack. Remaining: faint rebuilt dent on the apple next to the cap; a small joint smudge right of the pack base |

## Gooday design | competitor reference + stats | what we borrowed and changed
Source: **Justin's real TrendTrack screenshots** (`style-references/trendtrack-swipes-2026-11-27/`). Stats are read off the screenshots. Nothing is estimated.

Ad IDs are not visible in the screenshots, so there are no direct ad links. To find them, use TrendTrack → gruns.co / goli.com → Ad Library, or the Meta Ad Library search ([Grüns](https://www.facebook.com/ads/library/?active_status=active&ad_type=all&country=US&q=gruns), [Goli](https://www.facebook.com/ads/library/?active_status=active&ad_type=all&country=US&q=goli)).

**Honest note on "proven":** all three references are short runs so far (6 to 18 days). The only long runner in Justin's swipes is First Day "52% OFF / LAST CHANCE TODAY": 100 days, 11 variations, rank 7/2,834. It is discount and urgency led, so it is not usable for us. I picked the patterns Justin named (stat strip, apology hook, pack on real fruit).

| Gooday design | Competitor reference + stats | What we borrowed and changed |
|---|---|---|
| D1 "Here's your fibre." `run-0458/D1_B_HeresYourFibre.png` | **Grüns, "KEEP 💩 MOVING!"** sachets + gummies on a cream field with a stat strip "6g fiber \| 20 calories \| 0 sugar", Meta. Crop `refs/gruns-keepmoving-statstrip-swipe06.png`. TrendTrack (swipe-06, card 2): **active 18 days (9 Nov → now)**, rank **66/278 (24%)**, trending down, no targeting data, no variation count shown. Why it works: three checkable numbers in one compact strip; the pack is the hero. | Borrowed: a compact stat strip next to the pack. Changed: **Green claims only** ("6 g fibre", "no mixing", "no shaker"; no kcal, which is confirmed for green grape only). No poop or gut wording (gut lines are an Open question), no "0 sugar", no "prebiotic", and the body-symptom caption ("Bloating, sluggish digestion…") is not used (Meta and claims rules). Real photo of the founder's open palm instead of a studio flat lay; strip stacked vertically beside the pack. None of their words, pack or branding. |
| D2 "We're so sorry." `run-0458/D2_A_SoSorry.png` | **Grüns, "WE'RE SO SORRY"** fake-apology long-copy static, Meta. Crop `refs/gruns-weresosorry-swipe06.png`. TrendTrack (swipe-06, card 4): **active 6 days (21 Nov → now)**, rank **77/278 (28%)**, trending up, target US, no variation count shown. Why it works: an apology headline breaks the pattern, and the body pays it off. | Borrowed: the apology headline + short body that pays it off. Changed: **the apology is true**: it's not on sale yet. No discount, "make it right" offer, Black Friday or GLP-1 angle; no broccoli comparison (whole-food comparison is Open); no fire emojis or cursor graphics. No supply-timing words ("in development" per the 28 Nov rule); no kcal on collagen. Real photo scene, peach collagen pack. |
| D3 "Crunch now. Squeeze later." `run-0458/D3_B_CrunchNow.png` | **Goli, Beauty Stik "Make room for skin hydration."** jelly stick on a plate with real strawberries, Meta. Crop `refs/goli-beautystik-strawberry-swipe10.png`. TrendTrack (swipe-10, card 1): **active 10 days (17 Nov → now)**, rank **111/269 (42%)**, target US, no variation count shown. Sibling statics with the same pack-on-strawberry look in the same swipe ran 9 days (ranks 114 to 128/269). Why it works: a jelly pack next to its real flavour fruit says the flavour at a glance; calm, soft styling. | Borrowed: a jelly pack beside its real flavour fruit, with one bold line. Changed: Justin's own apple, table and hand (a real home scene, not a studio set); a two-beat headline that pairs the fruit with the pouch (no fruit-equivalence or nutrient comparison). No skin, hydration, hair or nails claims (Red for us). No coupon codes or "stack" offers (ACCC: no discount theatre). None of their words or branding. |

## Compliance self-check (against brain/claims.md, incl. Rules learned 27 and 28 Nov, and the coordinator's 28 Nov notes)

| Item | Line | Ruling |
|---|---|---|
| D1 headline | "Here's your fibre." | PASS. Format/offer line. No health, gut or dose claim, no "you have…" body language |
| D1 strip | "6 g fibre" / "no mixing" / "no shaker" | PASS (v4, after FIX). Green word for word. v3 had "about 25 kcal": that is confirmed for the green grape fibre pouch only, not green apple, so it was replaced |
| D2 headline + body | "We're so sorry." / "5 g collagen in a squeezable pouch. Peach flavour. No shaker. It's still in development, so you can't buy it yet." | PASS. Green "5 g collagen" + format; honest pre-launch statement; "in development" (no "coming soon" / "on its way"); no kcal on collagen; no skin, hair, joint or training link; no offer or urgency |
| D3 headline + subline | "Crunch now. Squeeze later." / "Green apple flavour. 6 g fibre per pouch." | PASS. "Squeeze" is a format word (Green "squeeze and go"); no claim that the pouch replaces or equals fruit. Reuse rule: never pair it with "an apple a day", "as good as an apple" or fruit-serve equivalence |
| All packs | "6 g fibre per pouch" / "5 g collagen per pouch", "Fibre + greens jelly" / "Collagen jelly", flavour, "Squeeze & go / No scoop, no shaker, no mixing" | PASS. "TEAR HERE" removed and "Tear" dropped (screw-cap shape); Net/kJ erased; Amber/open lines erased; the sugar/greens/Kakadu line is unreadable |
| All | Footer "Not on sale yet. Concept pack shown. Nutrition figures are targets…" on a dark scrim, readable on a phone | PASS (27 Nov rule; waitlist ads with concept renders, ACCC 128/26 rule) |
| All | Our spouted shape only, never the stand-in silhouette; normal fill; true-to-flat proportions; no jelly or texture shown | PASS (28 Nov AI/composited-image rule). Before pre-orders or any price: replace with photos of a real printed pack |
| All | No third-party branding, no competitor named, no before/after, no urgency, discount or "sold out", no licensed characters | PASS |

**Result: PASS (all three finals; D1 final = v4 after the kcal FIX).**

## Method notes (reusable; scripts in `run-0458/source/`)
1. **Perspective wood:** `oldshape/rowfill.py` fills from the same rows only, so the grain size and blur match the depth. Copying from far up the frame gave a blurred patch (depth of field). Give the board-joint line so the strip stops before it. Fill the fruit first, protecting the stand-in hole, then fill the stand-in.
2. **Skin:** `oldshape/shiftfill.py` (Telea light level + texture from a clean skin patch). Better still, tilt or shift the pack (`rot_deg`, `dx`) so its shoulder covers the hardest gap (here, between thumb and palm).
3. **Fruit under the stand-in:** `oldshape/applefix.py` rebuilds the edge (ellipse fit + skin fill + contact shadow); place the cap over the seam.
4. **woodfill.py fix:** high-pass grain inside the hole or protect mask is zeroed before sampling (it had copied stand-in and apple pixels).
5. **Print:** `real/fixflat.py` makes the `_k` flats (no "tear", "Squeeze & go", no Net/kJ). Use them for every old-shape render from now on.
6. **Shot tips for Justin:** the open-palm shot is the most premium-looking scene so far. A clean shot with the thumb clearly above the pack would avoid the gap fill. A green apple, and a peach, would still help.

## Question for Justin
Approve D1, D2, D3, any mix, or none? Approved designs go to `static-ads/approved/2026-11-28/` and the Miro "Approved ads" frame.
