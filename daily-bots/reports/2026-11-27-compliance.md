# Compliance bot: 27 Nov 2026 (morning)
Checked against `brain/claims.md` (25 Nov version + 2 rules added today), `brain/legal.md`, `brain/formulation.md` and the 24 to 26 Nov production rules. Scope: every draft and design made since the last report (`2026-11-26-compliance.md`, 25 Nov ~10 PM UTC). Planning guide, not legal advice. Marks: **PASS**, **FIX** (exact fix given) or **BLOCK**.

## Summary
| # | Item | Mark |
|---|---|---|
| 1 | Run-2231 D1 "Scoops are over." (`D1_A_ScoopsOver_real.png`) | **PASS** |
| 2 | Run-2231 D2 "Skip the glass." (`D2_B_SkipTheGlass_real.png`) | **FIX** (small print can't be read over the grapes) |
| 3 | Study headline 1 "Tear. Squeeze. Done." | **PASS** |
| 4 | Study headline 2 "Collagen, with Kakadu plum." | **PASS** (conditions) |
| 5 | Study headline 3 "Leg day? Peach day." | **FIX** (implies a recovery claim for collagen) |
| 6 | 27 Nov supplier follow-ups (8 emails + ATIQ website form) | **PASS** |
| 7 | Legal & admin bot 27 Nov output (report + legal.md section) | **PASS** + 1 note |

**Counts: 5 PASS, 2 FIX, 0 BLOCK.** Morning run-0458 designs (27 Nov): **pending**. The folder `static-ads/daily/2026-11-27/run-0458/` was still empty when this report was finished (about 5:05 AM Melbourne), so those designs need their own Compliance check before they go to Justin.

Not counted (already checked, unchanged): Bionutricia Gmail draft (PASS 26 Nov, optional "import compliance" tweak still open); Nam Viet reply (PASS 26 Nov, Justin sent it 26 Nov). Superseded files `D1_A_ScoopsOver.png` / `D2_B_SkipTheGlass.png` (pre-realism versions; same copy): **do not use**, the `_real` versions replace them.

## 1. Run-2231 ads (`gooday-launch/static-ads/daily/2026-11-26/run-2231/`)
| Design | Every line on the ad | Check | Mark |
|---|---|---|---|
| D1_A_ScoopsOver_real | "Scoops are over." / "5 g collagen jelly. Peach flavour." / pack: "gooday", "Collagen jelly", "5 g collagen per pouch", "Peach flavour" / "Join the waitlist" / "Not on sale yet. Concept pack shown. Nutrition figures are targets and will be confirmed before launch." | "Scoops are over" is a format line (Green "no mixing, no shaker"). It names no brand, makes no superlative and makes no health claim. "5 g collagen" is Green. "Peach flavour" appears twice, so the real peaches don't suggest fruit content. No skin, hair or beauty words or images. Lower pack panel (Amber "Marine collagen peptides", Kakadu, sugar line): full-size crop checked; blurred and can't be read. Small print sits on the dark lower area and is readable | **PASS** |
| D2_B_SkipTheGlass_real | "Skip the glass." / "6 g fibre jelly. Green grape flavour." / pack: "gooday", "Fibre + greens jelly", "6 g fibre per pouch", "Green grape flavour" / CTA / same small print | Copy: all Green ("Skip the glass" is a format line; "6 g fibre per pouch"). The lower pack panel is blurred and partly behind grapes; "Good source of fibre" (Amber) can't be read. **Problem:** the cream small print sits straight on pale green grapes. At full size it is faint; on a phone it can't be read. That line qualifies the "6 g" figure ("targets") and the pre-launch status ("Not on sale yet"). A qualifier that can't be read doesn't count (ACL s18/s29, ACCC fine-print guidance) | **FIX** |

**Exact fix for D2 (copy unchanged):** add a dark scrim behind the small print: a bottom gradient from transparent to black at 55% opacity over the lowest 170 px (y ≈ 1180 to 1350), so it sits under both the CTA pill and the small print. Keep the small-print text, size and colour as they are. Check by eye at 25% zoom that the line reads. D1 already has this contrast and needs no change. After this edit: **PASS**.

Notes for both (not marks):
- **Photo licences OK:** both background photos are CC0 Wikimedia Commons files (`source/PHOTO-CREDITS.txt`). Re-check the file pages before any paid run.
- **Pack art licence (all ads that show the pack, not new today):** `brain/product.md` says "fruit photos are mockup-only (licence)" for the fruit photos printed on the round 3 pack. That is fine for waitlist concept ads shown to Justin. Before any **paid** run, confirm or replace the printed peach and grape photos with licensed ones. Flag for Marketing and Justin.
- If the final collagen formula has no peach fruit, every peach ad must keep the word "flavour" next to "Peach" (both do now).

## 2. 3 headlines from `reports/2026-11-27-marketing-study.md`
| # | Headline + subline | Check | Mark |
|---|---|---|---|
| 1 | "Tear. Squeeze. Done." / "6 g fibre per pouch." (grape on teal) | Format line (Green "squeeze and go") + Green number. No claim | **PASS** |
| 2 | "Collagen, with Kakadu plum." / "5 g collagen per pouch." (peach on maroon) | Same meaning as the Green "Made with Kakadu plum". The line names no vitamin C or skin benefit | **PASS** with 3 conditions: (a) no vitamin C, "glow", skin or "Australian superfood" words or imagery on the ad, because Kakadu is known for vitamin C and the collagen formation claim is Amber; (b) Kakadu plum must stay in the chosen formula at a real amount (formula still Open in decisions.md; formulation.md warns that a tiny Kakadu share makes a Kakadu story misleading under ACL); (c) if the pack also puts Kakadu up front, the label must state its percentage (characterising ingredient, Std 1.2.10). Label point goes to the NIP sign-off |
| 3 | "Leg day? Peach day." / "5 g collagen per pouch. In your gym bag." (peach on charcoal) | "In your gym bag" is Green. But the headline links the **collagen** pouch to a specific workout. Collagen is sold everywhere for joints and recovery, so readers will take it as an implied "for leg-day recovery / joints / muscle" claim (Red: "faster recovery", "repairs joints", "builds muscle"). A protein-to-muscle claim would need "source of protein", which is still Open for 5 g collagen. Green allows the gym as a **place or bag moment**, not as the reason to take collagen | **FIX** |

**Exact fix for headline 3:** headline **"Gym bag? Peach packed."** with the subline **"5 g collagen per pouch. Squeeze and go."** Same peach-on-charcoal look. No legs, muscles, sweat, stretching or post-workout images. After this edit: **PASS**. (If Marketing wants a leg-day line, use it on the **fibre** SKU only, e.g. "Leg day? Grape day." / "6 g fibre per pouch. In your gym bag.", which carries no recovery link. Compliance must see it before use.)

## 3. 27 Nov follow-ups (`2026-11-26-procurement.md` §2, list in `2026-11-27-procurement.md`): PASS
I re-checked the final list after the ATIQ bounce:
- **8 emails (Litafood, Victory Foods, JoyGlo, SDFOOD, Sand-M, Nawon, Sunsho Trade, Thoyyib Pharma):** these are B2B enquiries. They make no health, gut, weight or comparative consumer claims. "Konjac-free" and "no inulin" are spec requests. The optional 10 g line is a sample request. No recipe detail beyond the approved 23 Nov RFQ (NDA rule in legal.md). Greeting lines (Chinese, Korean, Thai, Vietnamese) are neutral introductions. **PASS.**
- **Litafood ATIQ forward line:** ATIQ bounced for good, so the condition is met. Include it. It is factual. **PASS.**
- **Sand-M Jelly Me line:** it goes to Jelly Me's own maker, not into an ad. **PASS.**
- **ATIQ (#9):** off the email list. Pasting the **unchanged** approved 23 Nov RFQ into the ATIQ website form: **PASS**. Any new wording in the form needs a re-check.
- Still: **nothing goes out until Justin says go**, and Justin sends it himself. Bots never send.

## 4. Legal & admin bot 27 Nov output (`reports/2026-11-27-legal.md`, `brain/legal.md` "This week from Melbourne"): PASS
Internal admin guidance only. No customer-facing wording, no claims, nothing filed, signed or paid, labelled "not legal, tax or biosecurity advice". The Director ID number is kept out of the brain (correct). **PASS.**
- **Note (link to marketing):** legal.md now says the ~45 hand-carried Thai packs are for **tasting only, no resale or giveaways**. So the 26 Nov blind-tasting UGC brief and Content Script 1 must not let creators or guests take packs home. Add to the UGC brief: **"All imported sample packs stay with Gooday; no packs are given away or taken home."** This is a note on an already-fixed brief, not a new mark.

## 5. Other folders checked
- `daily-bots/` since 25 Nov ~10 PM UTC: new files are only the reports above, plus finance (no drafts), inbox (no drafts created) and PLAYBOOK.md (rules, not a draft). `daily-bots/legal/` has no new drafts.
- `static-ads/daily/2026-11-26/`: D1 to D3 (morning) were checked in the 26 Nov report. New since: run-2231 (above) and `refs/` (competitor screenshots, internal only, never published).

## 6. Rules learned today (added to brain/claims.md)
1. **Collagen and training:** collagen ads may use the gym only as a place or bag moment ("in your gym bag"). They must not tie collagen to a workout type or a post-training reason (leg day, "after legs"), because that reads as an implied recovery or joint claim.
2. **Small print on photo ads:** the qualifying small print ("Not on sale yet… targets…") must sit on a plain or darkened area and be readable on a phone. Busy photo backgrounds need a scrim.

## 7. Open questions for the consultant
None new. Existing Open items unchanged.

Brain updated: claims.md (2 rules in "Rules learned" + changelog line), changelog.md.
