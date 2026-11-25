# Marketing

## Ad test (status 22 Nov 2026: no results logged)
- Tracker: `../gooday-launch/gooday-ad-test-tracker.xlsx` (Daily log empty as of 22 Nov).
- Two angles: **A collagen** (peach, Kakadu plum) and **B superfood** (fibre + greens, green apple).
- First wave (8 ads, `../gooday-launch/static-ads/`): A-1 Minus the shaker, A-3 Gym bag, A-6 Tub in the cupboard; B-1 Ditch the powder, B-3 Hey it's OK, B-4 Your gut called, B-5 Swap the pile, B-6 Treat 25 kcal. Extra: B-9 to B-13.
- **Decision rules:** A$10 a day per ad, 7 days. Judge an angle after 150 landing page views. GO at 8%+ signup rate, STOP under 3%, keep testing in between. Pause an ad over A$20 cost per signup.
- On GO: send the manufacturer message for that angle (see [suppliers.md](suppliers.md)).
- Landing pages: `../gooday-launch/landing-page/` (not yet published on Netlify).
- Daily ad designs from the Marketing bot go to `../gooday-launch/static-ads/daily/<date>/`; only Justin-approved ones move to `approved/` and Miro.
- Short-video scripts and UGC briefs (Content bot, Mon/Wed/Fri): 24 Nov 2026 set (3 scripts on B-1, A-3, B-5/B-6 + 1 UGC brief; Content bot marked all PASS, but the 24 Nov Compliance check re-marked the 3 end cards, the Script 2 hook, the Script 3 pile-replacement shot and the UGC mock-up pack lines as FIX, see `../daily-bots/reports/2026-11-24-compliance.md`) in `../daily-bots/reports/2026-11-24-content.md`. Production rule (24 Nov): frame the round 3 pouch on its top half; the lower lines "Good source of fibre" (Amber) and "Marine collagen peptides" (collagen source still open) stay out of focus and out of copy. No eating or taste shots until real samples exist.
- Content set 26 Nov 2026 (Content bot, all PASS): Script 1 "What's out there. What we're making." (blind tasting of the Thai samples, founder-led), Script 2 "5 g collagen. Zero shaker." (motion), Script 3 "Pick your pouch. Fibre, squeezed." + UGC brief "Blind jelly tasting night" / "Say it bold": `../daily-bots/reports/2026-11-26-content.md`. Tasting-content rule (26 Nov): category samples decanted into numbered cups, no brands/packs/prices/sample numbers, no ranking or "ours is better", "Not Gooday" on screen, konjac samples off camera and never given away, Gooday mock-up never tasted.
- 25 Nov 2026 designs (all bold-statement led): D1 Number stack "6 g fibre. about 25 kcal. 0 scoops.", D2 Zero shaker "5 g collagen. Zero shaker.", D3 "Fibre, squeezed." All Compliance PASS (`../daily-bots/reports/2026-11-25-compliance-am.md`); waiting for Justin's approval.
- Pack in static ads (24 Nov 2026): round 3 pack images go through `../gooday-launch/static-ads/daily/2026-11-24/source/soften.py`, which soft-focuses the lower claim panel so it can't be read. 24 Nov designs (D1 What's in it, D2 Pick your pouch, D3 Big six) are all Compliance PASS and wait for Justin's approval: `../daily-bots/reports/2026-11-24-marketing.md`.

## Creators
- Mix to start: 2 to 3 dietitians, 4 to 6 micro fitness/wellness creators, 1 to 2 food reviewers. Gift first, unscripted, pay the ones that convert.
- Lists: `../market-research/gooday-audience-and-influencers-nov-2026.md` and the daily Marketing bot reports. Follower counts are estimates; check by hand before gifting.

## Agency
- Supplement Brand (supplementbrand.co, Lou Antonio). Playbook: customer, offer, page, ads. Notes: `../agency-call-prep/agency-client-review.md`.

## Justin to-dos (from Notion launch pack)
- Publish landing page and connect waitlist forms.
- Create Meta ad account and pixel, make one test signup.
- Phone clips or photos of a mock-up pouch.

## Competitor ad library
Long-running ads usually mean profitable ads. We adapt the idea (hook structure, layout, format) only: never their images, logos, mascots, exact wording or branding, and never name a competitor in an ad. Run lengths are from third-party trackers (Meta Ad Library pages block bots); treat as EST until checked by hand.

**23 Nov 2026 (Marketing bot)** · used in `../gooday-launch/static-ads/daily/2026-11-23/`, report `../daily-bots/reports/2026-11-23-marketing.md`

| Brand | Ad / link | Days running (EST) | Hook | Format | Why it works | Used in |
|---|---|---|---|---|---|---|
| Grüns | "Healthy Has Never Tasted So Good" [Meta 1505906931026556](https://www.facebook.com/ads/library/?id=1505906931026556); sibling "Delicious Nutrition in Every Bite" [Meta 2850815231931979](https://www.facebook.com/ads/library/?id=2850815231931979) | ~129 days each, ended ~Oct 2026 ([admakeai](https://admakeai.com/advertisers/gruns)) | Taste first, nutrition second | Not stated | Removes the "chore" objection; taste is the reason to start | D3 Make it peach |
| Grüns | "Struggling to Get Enough Fiber?" (several versions) [Meta 1016645160874260](https://www.facebook.com/ads/library/?id=1016645160874260), [1568451768213057](https://www.facebook.com/ads/library/?id=1568451768213057) | ~4 months, ended ~Oct 2026 ([admakeai](https://admakeai.com/advertisers/gruns)) | Fibre-gap question | Not stated | Names a common, simple gap. We can't copy the "Struggling…?" form (Meta personal attributes, claims.md) | Not used (rule) |
| Grüns | "13-in-1 daily immune support." [Meta 1707182057133923](https://www.facebook.com/ads/library/?id=1707182057133923) | 162 days, live since 27 May 2026 ([admakeai wrapped](https://admakeai.com/wrapped/gruns.md)) | Count-of-benefits number | Not stated | One big number reads at a glance. Benefit claims are Red for us; only the number-led layout is usable | Idea bank |
| Grüns | "F*CK YOU, HAIR LOSS." ([runneth/Motion library](https://runneth.com/library/gruns)) | Unknown (active) | Shouts directly at the enemy | Static, bright solid background, huge type, product | Loud pattern interrupt, one idea, product beside it | D1 Dear tub (direct address to the tub, warm not rude) |
| Grüns | "POV: you learn your collagen peptides need…" ([runneth](https://runneth.com/library/gruns)) | Unknown | POV knowledge gap | Static, UGC photo + text overlay | Looks native to the feed | Idea bank (needs real photo) |
| Grüns | Lisa Rinna "no time to take 25 pills… fits in my bag" ([runneth](https://runneth.com/library/gruns)) | Unknown | Pill fatigue + portability | Video, talking head | Relatable complaint; ends on the bag | Idea bank (our Green line: "Less to swallow than a pile of pills") |
| AG1 | "Every Woman Poops. Some Do It Regularly." 4 variants ([runneth/Motion library](https://runneth.com/library/ag1)) | Unknown (4 variants live suggests a winner) | Two-line contrast joke: universal line, then a twist | Static, two-line headline over lifestyle scene | Humour breaks supplement-ad sameness; second line lands the benefit | D2 Squeeze it in |
| AG1 | "Why women over 40 are switching to THIS" 5 variants ([runneth](https://runneth.com/library/ag1)) | Unknown | Curiosity + switching | Static, question + benefit icons + offer | Curiosity plus scannable icons | Idea bank ("switching" must not imply replacing supplements) |
| AG1 | Best ads ran over a year; hooks "4 reasons I drink this", "Why I quit my supplements for this" ([Foreplay](https://www.foreplay.co/post/athletic-greens-600m-ad-creative-strategy-how-foreplay-helps-you-dominate-the-market)) | 1 year+ (per Foreplay, ads not named) | Reasons listicle / switching story | Mixed | Reason-to-believe in a list | Not used ("quit supplements" = Red for us) |
| Vital Proteins | "Stay Vital. Stay You." [Meta 2721051364943435](https://www.facebook.com/ads/library?id=2721051364943435) | 168 days, 15 Apr to 30 Sep 2026 ([admakeai wrapped](https://admakeai.com/wrapped/vital-proteins.md)) | Short brand-name slogan | Not stated | Brand-led and easy to remember | Idea bank |
| Bloom | "Introducing the Creatine Gummies Mega Pack!" [Meta 1335901045013689](https://www.facebook.com/ads/library?id=1335901045013689) | 216 days, 12 Mar to 15 Oct 2026 ([admakeai wrapped](https://admakeai.com/wrapped/bloom-nutrition.md)) | "Introducing…" launch line | Likely static (76% of Bloom launches are static) | Simple launch news plus value pack | Idea bank (launch day) |

**24 Nov 2026 (Marketing bot)** · used in `../gooday-launch/static-ads/daily/2026-11-24/`, report `../daily-bots/reports/2026-11-24-marketing.md`

| Brand | Ad / link | Days running (EST) | Hook | Format | Why it works | Used in |
|---|---|---|---|---|---|---|
| AG1 | "Why women over 40 are switching to THIS", 5 variants ([runneth](https://runneth.com/library/ag1)) | Unknown (5 live variants) | Curiosity + callouts | Static, "Feature Benefit Pointout": product in the centre, icon/arrow callouts | Scannable reasons around the product | D1 What's in it (layout only; Green facts) |
| Bloom | Shirley Temple energy sticks statics, 7 of 14 live statics are pointouts ([runneth](https://runneth.com/library/bloom-nutrition)) | Unknown (most-used format) | Flavour + dose callouts | Static pointout | Dose, sugar-free and flavour at a glance | D1 (pattern proof) |
| Bloom | "Bundle & Save 15% / Fan-fave flavours" Splash Pack trio ([runneth](https://runneth.com/library/bloom-nutrition)); "Introducing the Creatine Gummies Mega Pack!" [Meta 1335901045013689](https://www.facebook.com/ads/library?id=1335901045013689) | Mega Pack 216 days, 12 Mar to 15 Oct 2026 ([admakeai](https://admakeai.com/wrapped/bloom-nutrition.md)) | Range in one frame + offer | Static, 3 flavours held together | Choice drives clicks; colour range stops the scroll | D2 Pick your pouch (no offer: not on sale) |
| Grüns | "13-in-1 daily immune support." [Meta 1707182057133923](https://www.facebook.com/ads/library/?id=1707182057133923) (already above) | 162 days | One giant number | Static | Number reads in 1 second | D3 Big six (quantity, not benefits) |
| Vital Proteins | "Stay Vital. Stay You." several IDs, e.g. [Meta 1275524488057256](https://www.facebook.com/ads/library/?id=1275524488057256) ([admakeai](https://admakeai.com/advertisers/vital-proteins)) | Up to ~5 months, ended Sep 2026 | Brand slogan | Not stated; live library is all video ([runneth](https://runneth.com/library/vital-proteins)) | Brand memory | Idea bank |

Not found today: long-running ads with run dates for Jelly Me, Everydaze or Physician's Choice (no tracker coverage). Check by hand in the Meta Ad Library (country AU and US).


**25 Nov 2026 (Marketing bot, Tuesday deep study: bold statements)** · report `../daily-bots/reports/2026-11-25-marketing-study.md`

| Brand | Ad / link | Days running (EST) | Hook | Format | Why it works | Used in |
|---|---|---|---|---|---|---|
| DAVID (protein, adjacent) | "28g Protein. 150 Calories. 0g Sugar." [Meta 921894010434469](https://www.facebook.com/ads/library/?id=921894010434469) | 203 days, 16 Mar to 6 Oct 2026 ([admakeai](https://admakeai.com/wrapped/david-protein.md)) | Three numbers, three full stops | Not stated | Checkable numbers = confident with no hype | Idea "6 g fibre. 25 kcal. 0 scoops." |
| Supergut (fibre) | "Increase Your Fiber Intake with Supergut" (5+ IDs, e.g. [Meta 1262350012760049](https://www.facebook.com/ads/library/?id=1262350012760049)) | ~3 months each, ended Jul 2026 ([admakeai](https://admakeai.com/advertisers/supergut)) | Plain imperative | Not stated | Clear job to be done; many versions = kept winning | Idea bank |
| Vital Proteins, Grüns, AG1 | see 23/24 Nov rows ("Stay Vital. Stay You." 168 days; "13-in-1" 162 days; "Every Woman Poops…" 4 variants) | | Two-beat slogan / one number / blunt contrast | | | Ideas "5 g collagen. Zero shaker.", "Fibre: yes. Shaker: no." |

Compliance 25 Nov: number-led bold lines PASS; never "most/highest fibre" (BLOCK).

Used 25 Nov (daily designs, `../gooday-launch/static-ads/daily/2026-11-25/`, report `../daily-bots/reports/2026-11-25-marketing.md`): DAVID number stack (203 days) → D1 Number stack; Vital Proteins two-beat slogan (168 days) → D2 Zero shaker and D3 Fibre, squeezed; Supergut plain statement (~3 months x5) → D3.

## Founder taste (24 Nov 2026)
- Justin: "we like bold statements". Approved D1 "What's in it. What's not." (callout/ingredient-transparency format). Marketing bot: lead with bold, short, confident headlines; make at least 2 of 3 daily designs bold-statement led. Approved later on 25 Nov: D2 Pick your pouch. Unapproved: D3 Big Six.
- Approved ads: static-ads/approved/<date>/ and Miro board https://miro.com/app/board/uXjVEOatDr0=/ (frame "Approved ads").
- 25 Nov: approved D2 Zero shaker (peach, maroon field, giant type) and D3 Fibre, squeezed (grape). Justin: "I don't like the apple ad" (D1 Number stack, apple). Avoid repeating that look; no reason given yet.
