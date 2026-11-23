# Marketing bot: daily designs
Tuesday 24 Nov 2026 (morning run). These are drafts only: nothing was posted, run, spent or sent.

Folder: `../../gooday-launch/static-ads/daily/2026-11-24/`. The finals are `D1_A_WhatsInIt.png`, `D2_B_PickYourPouch.png` and `D3_B_BigSix.png`; `_v1` and `_v2` are kept for comparison. Code is in `source/` there. Build steps: `python3 soften.py`, then `python3 daily.py v3 && node shot2.js`, run in a copy of `static-ads/source/` that has the pack PNGs.

**Pack:** round 3 only (`pouch-designs/final-with-critique/`): `pouch_v3_peach_collagen.png`, `pouch_v3_apple_fibre.png`, `pouch_v3_peach_fibre.png`, `pouch_v3_grape_fibre.png`. The `bag_*.png` files were prepared but not used today.
**Unconfirmed pack lines:** `soften.py` puts the lower panel of every pack image in soft focus (pouch y 960 to 1175 px, bag y 975 to 1150 px, Gaussian blur r16, alpha kept). That panel holds "Good source of fibre" / "Marine collagen peptides", the "plus greens · under 2 g sugar" line, "Tear, squeeze & go" and the net/kJ line. **I checked: none of it can be read**, even on the full 1080 px file. Flavour names and the top half ("5 g collagen per pouch", "6 g fibre per pouch") stay sharp.
**Small print on all three:** "Not on sale yet. Concept pack shown. Nutrition figures are targets and will be confirmed before launch."
**Not repeated from 23 Nov:** no break-up letter, no two-line contrast joke, no taste-first headline.

Scores run from 1 to 5, in this order: scroll-stop / one message / product visible / thumbnail-readable / on-brand / CTA / believable.

## Competitor study (today)
Run lengths come from third-party trackers. The Meta Ad Library blocks bots, so treat them as EST.
- **AG1, "Why women over 40 are switching to THIS"**: a "Feature Benefit Pointout" static, 5 live variants ([runneth/Motion library](https://runneth.com/library/ag1)). The product sits in the centre with icon and arrow callouts around it. Many live variants suggests a winner.
- **Bloom**: "Feature Benefit Pointout" is its most common static format, 7 of 14 live statics (Shirley Temple sticks: callouts for dose, sugar-free, flavour) ([runneth](https://runneth.com/library/bloom-nutrition)).
- **Bloom**: flavour-trio statics, "Bundle & Save 15% / Fan-fave flavours" Splash Pack, with three flavours held up together ([runneth](https://runneth.com/library/bloom-nutrition)). Also "Introducing the Creatine Gummies Mega Pack!" [Meta 1335901045013689](https://www.facebook.com/ads/library?id=1335901045013689), a static that ran **216 days** (12 Mar to 15 Oct 2026, [admakeai](https://admakeai.com/wrapped/bloom-nutrition.md)).
- **Grüns, "13-in-1 daily immune support."** [Meta 1707182057133923](https://www.facebook.com/ads/library/?id=1707182057133923), **162 days**, live since 27 May 2026 ([admakeai](https://admakeai.com/wrapped/gruns.md)). One huge number carries the ad (already in the idea bank).
- Vital Proteins: its live statics are all "Stay Vital. Stay You." brand lines (up to ~5 months), and its live library is video only ([runneth](https://runneth.com/library/vital-proteins)). Not used.
- Found nothing for Jelly Me, Everydaze or Physician's Choice (no tracker coverage). Check by hand in the Ad Library.
Logged in `brain/marketing.md` → "Competitor ad library", 24 Nov.

## D1_A_WhatsInIt.png (Angle A, collagen, peach)
- **Copy:** "What's in it." (maroon) / "What's not." (white). Callouts with dotted arrows: "5 g collagen per pouch", "made with Kakadu plum", "<2 g sugar", "~35 kcal". Crossed-out chips: "Scoop", "Shaker", "Mixing". CTA "Join the waitlist".
- **Pattern adapted:** the **Feature Benefit Pointout** static (AG1 "Why women over 40 are switching…", 5 variants; Bloom's most-used static, see above). We kept only the layout: product in the centre, callouts with arrows. We added an in/out twist ("what's not" = the routine you skip) and dropped their benefit callouts, since we only use Green facts. No wording, images or branding from their ads.
- **v1: 3/3/5/3/4/4/5.** Flaws: the plain headline "What's in the pouch." gives no reason to stop; the callouts float without arrows, so they read as random numbers; the calm cream page and small text are weak at thumbnail size.
- **v2: 3/4/5/3/4/4/5.** Changes: the in/out headline, dotted arrows, crossed-out chips and a peach glow. Flaws: the arrowheads were huge and landed on the pack's own "5 g collagen" text; the Kakadu label "plum in the mix" read oddly; the cream background still felt flat.
- **Final (v3): 4/5/5/4/4/4/5.** Changes: a full peach radial background, "What's not." in white, arrows that stop at the pouch edge with smaller heads, and the Kakadu note rewritten as the Green wording "made with Kakadu plum".

## D2_B_PickYourPouch.png (Angle B, fibre, three flavours)
- **Copy:** "Pick your pouch." / "Three flavours. 6 g fibre in each." / pouches in green apple, peach and green grape, fanned / colour-dot chips with the flavour names / CTA "Join the waitlist".
- **Pattern adapted:** Bloom's **flavour-trio** static (Splash Pack, "fan-fave flavours"), with the 216-day "Mega Pack" static as proof that a range-in-one-frame works. We can't make an offer (not on sale), so the "save" became a choice ("pick your pouch"). Nothing copied.
- **v1: 3/4/5/4/4/3/5.** Flaws: three upright pouches in a row look like a catalogue page; the headline and flavour names compete; the CTA doesn't link to the "pick" idea.
- **v2: 3/4/5/4/4/4/5.** Changes: the pouches are fanned and overlap with the middle one forward, with dot chips for flavours. Flaws: the subline was squeezed beside the headline; the light background is still too calm to stop the scroll; the grape pack's "6 g" was hidden.
- **Final (v3): 4/5/5/4/4/4/5.** Changes: a solid green header with a curved edge and a one-line white headline, the subline on its own row, and bigger pouches.
- Note: peach fibre and the grape colour are open decisions (decisions.md, 21 Nov). If peach fibre is dropped, swap that pouch out.

## D3_B_BigSix.png (Angle B, fibre, green apple)
- **Copy:** a giant "6g" / "of fibre in one squeeze-and-go pouch." / chips "About 25 kcal", "Under 2 g sugar", "No mixing, no shaker" / CTA "Join the waitlist".
- **Pattern adapted:** Grüns' **number-led static** "13-in-1 daily immune support." (162 days EST). One huge number carries the ad. We swap the benefit count for a quantity fact (Green) and add no benefit claims.
- **v1: 4/4/4/4/4/4/5.** Flaws: "6 g" and "fibre per pouch." are two separate ideas fighting each other; the pouch is small and far right; the bottom third is empty.
- **v2: 4/5/5/5/4/4/5.** Changes: the number is bigger with a green "g", the line "fibre in one squeeze-and-go pouch." is bolder, a third chip was added, and the pouch is bigger. Flaw: the copy started "fibre in…", which reads as a fragment after "6g".
- **Final (v3): 5/5/5/5/4/4/5.** Changes: the copy now reads "of fibre in one…", the number is bigger, and a white glow sits behind the pouch.

## Claims self-check (Compliance bot result in `2026-11-24-compliance.md`)
All the copy is Green wording from claims.md. There is no gut, skin, weight, GLP-1 or "superfood"/"daily greens" wording, no "you" statements and no competitor names. The pack lower lines are not legible. **Compliance: all 3 PASS** (see the compliance report).

## For Justin
Which designs do you approve: D1, D2, D3? Only approved ones go to `approved/` and Miro.
