# Compliance bot (gatekeeper): review of drafts to date
Monday 23 Nov 2026 (prepared 22 Nov). Review only: nothing was posted, sent or changed in the drafts. **Not legal advice.** These are planning checks against brain/claims.md (master copy of the Claims sheet) and the FSANZ notes in `2026-11-22-research.md`. The regulatory consultant has the final say.

**Rules used:** FSANZ Std 1.2.7 + Schedule 4 (content and health claims, NPSC), Std 1.3.2 + Schedule 17 (no added vitamins in jelly), TGA food-medicine interface (no dose, "take" or therapeutic wording), Australian Consumer Law ss 18 and 29 (misleading claims, testimonials, ACCC influencer guidance), Meta ad policy (no before and after, no implied personal attributes, health claims).

## Scorecard

| Group | Items | PASS | FIX | BLOCK |
|---|---|---|---|---|
| 1. Creator DMs (marketing, 22 Nov) | 5 | 2 | 3 | 0 |
| 2. Consultant email (research, 22 Nov) | 1 | 1 | 0 | 0 |
| 3. RFQ + Sand-M email (procurement, 22 Nov) | 2 | 0 | 2 | 0 |
| 4. Static ads (14 PNGs, ads.py + wave2.py) | 14 | 6 | 8 | 0 |
| 5. Landing pages | 2 | 0 | 2 | 0 |
| **Total** | **24** | **9** | **15** | **0** |

Nothing is BLOCKed: no weight-loss, drug (GLP-1), before-and-after or therapeutic claims were found. Under the playbook, the 15 FIX items are **not ready** until the fixed wording is in.

**Top 3 fixes**
1. **B5 "Swap the pile for one pouch."** (pills, tubs, scoops into one pouch) implies Gooday replaces supplements. The landing pages repeat the idea in "no pile of pills". Use the Green line "Less to swallow than a pile of pills."
2. **Superfood landing page: "Your daily greens, in one squeeze."** About 2 g of greens is under a quarter of one vegetable serve (nutritionist report), so "daily greens" can mislead (ACL s18). Also the superfood FAQ says "gelatin set", but that line is vegan (pectin or gellan).
3. **Supplier drafts describe the product wrongly.** The RFQ asks for "inulin or FOS" fibre and "marine preferred" collagen; product.md says resistant dextrin or soluble corn fibre + apple pectin, and the collagen source is undecided. "Kakadu plum (vitamin C)" and "plus vitamin C" must say *naturally occurring, no added ascorbic acid* (Std 1.3.2). This matters most for Sand-M, whose own versions are sold as dietary supplements with added vitamins.

---

## 1. Creator DMs (`2026-11-22-marketing.md`)

The general check is fine: the DMs state amounts, taste and format only, with no health outcomes. The problems are disclosure and accuracy.

| # | Creator | Mark | Problem line | Fix | Rule |
|---|---|---|---|---|---|
| 1 | @healthybodhealthymind | **PASS** | | Depends on: "6 g fibre", "about 25 kcal" (targets) | |
| 2 | @julzhealth | **FIX** | No disclosure line. "we'd chat about a proper paid collab" | Add: "If you do post, please tag it #gifted (or #ad if paid), and we'll send a short list of what we can and can't say about it." | ACL s18, ACCC influencer guidance (the brand shares liability for undisclosed promotion), AANA Code 2.7 |
| 3 | @alpendlebury | **FIX** | No disclosure line | Add the same disclosure sentence. Also say "one pouch a day" rather than implying a routine she needs | ACCC influencer guidance |
| 4 | @lucyisdewy | **FIX** | "5 g marine collagen" | "5 g collagen" (bovine or marine is still undecided, product.md) | ACL s29(1)(a): the composition must be accurate |
| 4 | | | "that replaces the scoop in your coffee" | "no scoop or mixing needed" | Keeps it a format point rather than a product-equivalence claim |
| 4 | | | No disclosure, and she is a skincare creator | Add the disclosure sentence plus: "We can't make skin claims for collagen in Australia, so we'd keep it to taste and format." | No collagen skin claim exists (Sch 4); the brand is liable for creator claims |
| 5 | @livfozz | **PASS** | | Depends on: "No fridge" (12-month ambient shelf life is still only an ask), and kcal targets | |

## 2. Consultant email (`2026-11-22-research.md`): **PASS**

It is internal-facing and only asks questions; it does not promise any claim. Two small notes, and no change is needed to send:
- "Collagen + Kakadu plum (natural vitamin C)" works as a description. Don't carry "natural vitamin C" onto the pack or ads until the consultant rules (ACCC guidance on "natural").
- Worth adding to the email: the new consultant questions listed below (superfood name, "daily greens", 5 g collagen vs the 5 g *protein* threshold, influencer briefs).

## 3. Supplier drafts (`2026-11-22-procurement.md`)

**3a. Draft RFQ: FIX** (accuracy against product.md)

| Problem line | Fix | Why |
|---|---|---|
| "6 g prebiotic fibre (inulin or FOS)" | "6 g fibre (resistant dextrin or soluble corn fibre, plus apple pectin; please also quote acacia fibre)" | product.md spec; inulin and FOS are high-FODMAP (nutritionist 1.3). "Prebiotic" is claim-type language, so keep it off the spec. |
| "5 g collagen peptide (marine preferred)" | "5 g hydrolysed collagen peptides; please quote bovine and marine (and say if halal)" | The source is an open decision (decisions.md). Marine means a fish allergen declaration. |
| "Kakadu plum (vitamin C)" | "Kakadu plum powder as a whole-food ingredient. No added vitamins or ascorbic acid. Please state the natural vitamin C per serve at end of shelf life." | Std 1.3.2 / Sch 17: jelly can't carry added vitamins |
| "sold as a food in Australia" | Keep, and add: "general food, not a dietary supplement or sports food" | Keeps the factory from proposing supplement formats or doses |

The format (a 20–30 g stick or a small pouch, quote both) is fine to ask about because the format is an open decision. product.md still says 120 g spout pouch.

**3b. Sand-M email: FIX**

| Problem line | Fix | Why |
|---|---|---|
| "2. Collagen and Kakadu plum: about 5 g collagen peptide plus vitamin C" | "about 5 g collagen peptide with Kakadu plum (vitamin C only from the fruit itself, no added vitamins)" | Std 1.3.2. Sand-M's collagen stick has vitamin C added as a Thai supplement. |
| "Fibre and greens: about 6–7 g fibre ..., greens, 0 g added sugar" | "... greens (about 2 g), under 2 g sugar, sweetened with stevia or monk fruit" | Match product.md (under 2 g sugar). Erythritol is under review (nutritionist 1.5). |
| "a new Australian wellness brand launching single-serve functional jelly sticks" | Add one line: "In Australia these are sold as a general food, not a dietary supplement." | Their range is registered as supplements in Thailand, so avoid copying that model |

---

## 4. Static ads (`gooday-launch/static-ads/*.png`, copy from `source/ads.py` and `source/wave2.py`)

| Ad (PNG) | Headline / copy | Mark | Fix and rule |
|---|---|---|---|
| A_A1_NoShaker | "Your collagen, minus the shaker." / "Clumps in your coffee", "5 g collagen", "No mixing" | **PASS** | Green (format, collagen amount) |
| A_A3_GymBag | "Collagen for your gym bag." / 5 g collagen, ~35 kcal, No shaker | **PASS** | Green ("In your gym bag" as a moment) |
| A_A6_TubCupboard | "Collagen tub still in the cupboard?" / One a day, Fits in your bag | **PASS** | Green |
| A_A7_Consistency | "**Stopped taking your collagen?** Make it a treat." | **FIX** | "Taking your collagen" is supplement and dose language (TGA FMIGT), and it implies the viewer's habits. Use: **"Collagen you'll look forward to. Make it a treat."** |
| B_B1_DitchPowder | "Ditch the powder. Keep the daily habit." / 6 g fibre + greens, Tear and squeeze | **PASS** | "Tear and squeeze" depends on the stick format (the current spec is a spout pouch) |
| B_B3_HeyItsOK | "Forgot your daily scoop again? Hey, it's OK. One pouch a day." | **PASS** | Green ("One pouch a day") |
| B_B4_GutCalled | "**Your gut called. It wants more fibre.**" | **FIX** | This links fibre to a gut benefit, which is an implied general-level health claim (Std 1.2.7). Gut claims are Amber at best. Use the Green line: **"Made for your daily fibre habit."** Or: "Your fibre habit, made easy." |
| B_B5_SwapPile | "**Swap the pile for one pouch.**" / THE PILE: Pills, tubs, scoops | **FIX** | Implies it replaces supplements (Red: "Replaces your multivitamin"; ACL s18; TGA comparison). Use: **"Less to swallow than a pile of pills."** Keep the visual, and change the left label to "Lots to swallow". |
| B_B6_TreatCalories | "Tastes like a treat." / big "**25** kcal a pouch" | **FIX** (minor) | Green is "About 25 kcal" until tested. Use **"~25 kcal a pouch"** (add "about" or "~"). |
| B_B9_Broccoli | "Can't face 2½ cups of broccoli? **Get the same fibre in one squeeze.**" / footnote cites USDA | **FIX** | "The same fibre" suggests the same benefit as whole broccoli (ACL s18). Use: **"Get about the same amount of fibre (6 g) in one squeeze."** Use an Australian source (FSANZ Australian Food Composition Database) and check the per-cup figure. The comparison itself goes to the consultant. |
| B_B10_GreyTub | "Sick of clumpy greens powder? Get 6 g fibre. No shaker." | **PASS** | Green. Depends on 6 g. |
| B_B11_NotesApp | Phone-note style "Getting enough fibre: what I've tried", with "One gooday pouch with my coffee" ticked as done | **FIX** | It reads like a real person's experience of a product that doesn't exist yet: an implied testimonial (ACL ss 18, 29(1)(e); Meta). Retitle **"Getting more fibre: the easy list"**, change the ticked line to **"One gooday pouch (coming soon)"**, and keep the brand name visible. |
| B_B12_Doodle | "**Falling short on fibre?** Here's the easy way." / "no fridge needed", "fits in your pocket", "tear here" | **FIX** | The question implies something about the viewer's diet (Meta personal attributes; claims.md "for people who…" rule). Use: **"More fibre, the easy way."** "No fridge needed" depends on a 12-month ambient shelf life; "tear here" depends on the stick format. |
| B_B13_EasyWay | "**Falling short on fibre?** Here's the easy way." / Tear & squeeze, 6 g fibre in every pouch, Tastes like a treat, Fits in a pocket | **FIX** | Same as B12: **"More fibre, the easy way."** The format and 6 g caveats apply. |

The preview composites (`_all-*.png`, `_middle-ground-B13.png`, `_research-wave-preview.png`) are internal contact sheets of the same ads, not separate ads.

## 5. Landing pages

**5a. `landing-page/collagen/index.html`: FIX**
- The JS copy (angle a) is fine: "Collagen without the mixing.", "5 g of collagen with Kakadu plum …, about 35 kcal", "In your gym bag … Have it after training", "<2 g sugar", "(planned)" note and the footer disclaimer are all Green or properly hedged.
- **Problem:** the static HTML (shown before JS runs, and to crawlers including Meta's ad review) carries the **superfood** headline and lede: "Your daily greens, in one squeeze. … 6 g of fibre and greens, at about 25 kcal." A collagen ad would then land on fibre claims. Fix: put the collagen headline and lede in the static HTML.
- Depends on: "No fridge" (shelf life), "Tear, squeeze, done" (format), "Kakadu plum" (fine as an ingredient statement; no vitamin C claim is made, which is correct).

**5b. `landing-page/superfood/index.html`: FIX**
- "**Your daily greens, in one squeeze.**" → **"Fibre + greens, in one squeeze."** About 2 g of greens isn't a day's greens (ACL s18; nutritionist 1.4).
- FAQ "We use a soft fruit-pectin **or gelatin** set" → **"a soft fruit-pectin or gellan set (plant-based), not konjac."** product.md says this line is vegan.
- "Swap the pile: Less to swallow than a handful of pills and a scoop." PASS (Green). The lede "no pile of pills" is OK as format.
- Page title and angle name "Superfood": internal title only, so OK for now, but see the consultant question below before using "superfood" in customer copy.
- Both pages: the konjac FAQ with "Squeeze slowly, … not suitable for children under 5" matches the pack warning. Good.

---

## Claims that depend on unconfirmed formulation

| Claim used | Depends on | Status |
|---|---|---|
| "6 g fibre" (ads, DMs, pages) | Lab NIP; 6 g may be hard in a 20–30 g pectin stick (Sand-M note) | Target. Always keep "(planned)" on the pages. "Good source of fibre" (4 g+) is still Amber. |
| "5 g collagen" | Spec | Target. 5 g of collagen peptides is about 4.5 g of *protein*, so it may **not** meet "source of protein" (5 g protein per serve). The nutritionist and research reports disagree (10 g vs 5 g), so this goes to the consultant. |
| "~25 kcal" / "~35 kcal" / "<2 g sugar" | Lab NIP; the fibre and polyol energy factors | Target. Keep "about" or "~". |
| Kakadu plum vitamin C (any future claim) | At least 10% RDI (4 mg) **naturally present at end of shelf life**; no ascorbic acid | Not claimed anywhere yet, which is correct. Vitamin C breaks down with heat and over shelf life. The nutritionist assumes 40 mg+ in *both* lines, but product.md has Kakadu plum on collagen only. Align this. |
| "No fridge", "shelf-stable" | 12-month ambient shelf life (still only an ask) | Unconfirmed |
| "Tear and squeeze", "tear here" | Stick format (open decision; the spec is still a 120 g spout pouch) | Unconfirmed. Swap to "squeeze and go" (Green) if the pouch wins. |
| "Fits in your pocket" | Format and size | OK for a stick; a stretch for 120 g |
| Gel "pectin or gelatin" | Line: superfood is vegan (pectin or gellan) | See fix 5b |

## New questions for the consultant
Added under "Open" in `brain/claims.md`; no existing rulings were changed.

---
_Compliance bot. Not legal advice. Rulings are provisional until the regulatory consultant confirms them._
