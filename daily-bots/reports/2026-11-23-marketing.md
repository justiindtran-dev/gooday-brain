# Marketing bot: daily designs
Monday 23 Nov 2026 (prepared 22 Nov). These are drafts only: nothing was posted, run, spent or sent.

Folder: `../../gooday-launch/static-ads/daily/2026-11-23/`. Finals are `D1_A_DearTub.png`, `D2_B_SqueezeItIn.png` and `D3_A_MakeItPeach.png`. The v1 and v2 files are kept for comparison. The design code is in `source/daily.py` there; it runs inside a copy of `static-ads/source/`, with `python3 daily.py v3 && node shot2.js`.
Competitor ads studied are logged in `../../brain/marketing.md` under "Competitor ad library".

Scores run from 1 to 5, in this order: scroll-stop / one message / product visible / thumbnail-readable / on-brand / CTA / believable.

## D1_A_DearTub.png (Angle A, collagen, peach)
- **Copy:** "Dear collagen tub," (handwritten) / "It's over." (huge, white) / "5 g collagen in a peach jelly pouch." / chips "No scoop, no shaker" and "Squeeze and go" / CTA "Join the waitlist".
- **Inspired by:** Grüns' loud headline static "F*CK YOU, HAIR LOSS." ([runneth/Motion library](https://runneth.com/library/gruns)). It talks straight at the enemy in huge type on a bright solid colour, with the product beside it. Our version keeps the structure (direct address to the enemy) and makes it warm: a break-up note to the collagen tub instead of swearing. It uses no wording, colours or images from their ad.
- **v1:** 4/3/3/2/3/4/4. Flaws: the all-caps headline wrapped to 4 lines and ran into the subcopy; the peach pouch sat on the same flat peach background and disappeared; the shouty caps felt aggressive rather than warm.
- **v2:** 5/4/4/4/4/4/4. Changes: a Caveat "Dear collagen tub," over a 2-line "It's over.", a radial gradient, chips, and a bigger pouch. Remaining flaws: the peach fruit covered the pack text, and "now comes in a pouch" implied the product is on sale.
- **Final (v3):** **5/4/4/4/4/4/4**. Changes: the line now says "5 g collagen in a peach jelly pouch." (no "now available" hint), the peach fruit moved off the pack, and a cream glow sits behind the pouch for contrast.
- **Claims check (mine; still needs the Compliance bot):** "5 g collagen" Green; "No scoop, no shaker" matches Green "no mixing, no shaker"; "Squeeze and go" Green. It takes aim at a generic tub, never a brand. Watch: the "It's over" swap is a format swap (collagen for collagen) with the same logic as A6 (PASS). It does not say it replaces supplements.

## D2_B_SqueezeItIn.png (Angle B, fibre + greens, green apple)
- **Copy:** "Everyone plans to eat more fibre." (muted) / "Some just squeeze it in." (big, green punchline) / chips "6 g fibre per pouch", "About 25 kcal", "No mixing, no shaker" / CTA "Join the waitlist".
- **Inspired by:** AG1's "Every Woman Poops. Some Do It Regularly." (4 variants, [runneth/Motion library](https://runneth.com/library/ag1)). The pattern is a two-line contrast joke: a universal truth, then a twist that lands the product. Our version keeps the hook structure only; there is no body or gut-outcome claim, and the pun is on "squeeze".
- **v1:** 3/4/4/4/4/4/4. Flaws: both headline lines had the same weight, so the punchline didn't land; the chips overlapped the pouch edge; the bottom right felt empty.
- **v2:** 4/5/4/4/4/4/4. Changes: line 1 muted, line 2 at 132 px with "squeeze it in." in green, a third chip, and an apple. Remaining flaws: the CTA bar cut off the bottom of the pouch, and the apple covered the pack's kcal and fibre text.
- **Final (v3):** **4/5/5/4/4/4/4**. Changes: the pouch is smaller and sits fully above the CTA, and the apple moved under the chips so the whole pack is visible.
- **Claims check:** "6 g fibre per pouch" Green, "About 25 kcal" Green, "No mixing, no shaker" Green. There is no gut or benefit wording and no "you" statement about the viewer's body (it avoids the B12/B13 "Falling short on fibre?" FIX). Watch: Compliance should confirm "Everyone plans to eat more fibre" reads as a playful general line, not an implied personal attribute.

## D3_A_MakeItPeach.png (Angle A, collagen, peach)
- **Copy:** "Collagen, but make it peach." / stat bar "5 g collagen · ~35 kcal · <2 g sugar" / CTA "Join the waitlist".
- **Inspired by:** Grüns' taste-first statics "Healthy Has Never Tasted So Good" ([Meta 1505906931026556](https://www.facebook.com/ads/library/?id=1505906931026556)) and "Delicious Nutrition in Every Bite" ([Meta 2850815231931979](https://www.facebook.com/ads/library/?id=2850815231931979)), each ~129 days EST ([admakeai](https://admakeai.com/advertisers/gruns)). The pattern leads with taste and puts the nutrition numbers second. We avoided "healthy" (claim risk) and used flavour plus Green numbers.
- **v1:** 3/4/4/3/4/4/4. Flaws: the chip row covered the pouch's "5 g" badge; there was a big dead gap between the headline and the pouch; the calm cream page had low stopping power.
- **v2:** 3/4/5/5/4/4/4. Changes: a white 3-number stat bar, the pouch above it, and "peach." in accent colour. Remaining flaws: still too calm to stop the scroll (scroll-stop under 4, so a v3 was required), and the headline touched the pouch cap.
- **Final (v3):** **4/4/5/5/4/4/4**. Changes: a saturated peach top panel with a curved edge, a white headline with "peach." in dark ink, the pouch breaking out of the panel on the right, and larger peaches on the split line.
- **Claims check:** "5 g collagen" Green, "~35 kcal" Green ("about"), "<2 g sugar" matches Green "under 2 g sugar". There is no skin, hair or protein claim, and Kakadu plum isn't mentioned, so no vitamin C implication.

## Compliance: PASS after small-print fix
The Compliance bot marked all 3 finals FIX because the nutrition numbers are targets. The small print on D1_A_DearTub.png, D2_B_SqueezeItIn.png and D3_A_MakeItPeach.png now reads exactly: "Not on sale yet. Concept pack shown. Nutrition figures are targets and will be confirmed before launch." Nothing else changed, and the tub stays generic with no brand. All three were re-rendered, the finals in the folder were overwritten, and each was checked: the line fits on one row and is legible. **Compliance: PASS after small-print fix.**

## Shared notes
- All three carry the updated small print (see above) and the 120 g spout-pouch render (it matches product.md). None of them use "tear", "pocket" or "no fridge" (all unconfirmed).
- Avoided per yesterday's compliance report: "replaces/swap the pile", "your daily greens", "taking your collagen", gut-benefit jokes, "Falling short…?" questions, and "superfood".
- Peach and apple fruit renders come from the existing source assets. Check their licence before paid use (see PHOTO-CREDITS.txt).
- **Next:** the Compliance bot gives a PASS/FIX on the three finals. Then Justin picks which to approve; only approved designs go to `approved/` and Miro.
