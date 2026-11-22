# Gooday packaging: design and self-critique (21 Nov 2026)

Review page: https://claude.ai/artifact/DPNZbptTf8ceVDHqXwhJ2z

## Final (round 3)
- Pouch fronts: pouch_v3_apple_fibre.png, pouch_v3_peach_fibre.png, pouch_v3_grape_fibre.png, pouch_v3_peach_collagen.png (board: pouch-fronts-final.png)
- Pouch backs: pouch_v3_back_apple_fibre.png, pouch_v3_back_peach_collagen.png (board: pouch-backs-final.png)
- Outer bags (14 pouches): bag_apple_fibre.png, bag_grape_fibre.png, bag_peach_collagen.png (board: outer-bags-final.png)
- Tests: thumbnail-shelf-test.png (90 px thumbnail, blur, greyscale; round 1 vs round 3)
- Earlier rounds: rounds/round1-pouches.png, rounds/round2-pouches.png
- Source: source/design.py (pouch fronts v1-v3 + back panel), source/bagv3.py, shading scripts. Render: `python3 design.py v3 && node shot.js && python3 shade.py` (needs fonts.css, fonts/, flat.py, shade_core.py and fruit PNGs from static-ads/source and pouch-designs/source).

## Scorecard
| Must communicate | Round 1 | Round 2 | Round 3 |
|---|---|---|---|
| What it is | Fail: descriptor tiny, fruit covered it | Weak: pill added, fruit still overlapped | Pass |
| Benefit | Fail: slogan bigger than 6 g, no greens | Weak: white 6 g ~2:1 contrast | Pass: 6 g fibre in dark ink, "plus greens" |
| Flavour | Fail: apple and grape same green | Pass | Pass |
| Format | Weak: "ready to eat" only | Pass: tear, squeeze & go pictogram | Pass |
| Trust | Weak: kcal only, no smile link to bag | Weak: no back panel | Pass: NIP, ingredients, allergen, warning |
| Shelf/scroll | Fail: apple/grape merge at thumbnail | Fail: peach fibre = peach collagen | Pass |
| Claims | Weak | Weak | Needs regulatory review |

## Claims on final pack (my reading of FSANZ 1.2.7, not legal advice)
- "6 g fibre per pouch": nutrition content claim; fibre in NIP (done).
- "Good source of fibre": threshold believed to be >=4 g/serve; confirm.
- "Under 2 g sugar": must match lab NIP; avoid "low sugar"/"no added sugar" unless qualified.
- "Plus greens": declare greens % in ingredients.
- "5 g collagen": quantity only; no beauty/skin claims. Declare fish allergen.
- Left off: gut health, energy, immunity, recovery, beauty, weight, "Australian owned" (until confirmed).
- Earlier bag's "Energy · Immunity · Recovery · Beauty" should be removed; "Feel good again" implies a health outcome.

## Still falls short
1. Teal grape may read as mint; if tests show confusion, use red/purple grape.
2. Peach on both lines; consider fibre in apple + grape, peach for collagen only.
3. Apple and peach same tone in greyscale; flavour name carries it.
4. Smallest back-panel text ~2 mm at ~95 mm pouch width; print proof at real size; check net-weight minimum heights.
5. 14 x 120 g = 1.68 kg per bag; confirm pouch size for shipping.
6. Fruit photos are mockup-only (GFDL, photographer asks for commercial arrangement); grape photo uncredited.
7. Film shine crosses "fibre" on some renders (mockup lighting only).
8. Earlier bags say 14 and 28 pouches; pick one.
