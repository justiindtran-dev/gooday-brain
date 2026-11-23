# Compliance bot (gatekeeper): 24 Nov 2026
Morning run, Tue 24 Nov. Review only: **not legal advice**, nothing was posted, sent or changed in the drafts. Checked against brain/claims.md (23 Nov version), FSANZ Std 1.2.7 / 1.3.2, the TGA food-medicine interface, ACL ss 18 and 29 (incl. implied testimonials), Meta ad policy, and the NDA timing rule in brain/legal.md.

**Scope:** everything drafted since `2026-11-23-compliance.md`:
- today's 3 ads
- the 24 Nov content set (3 scripts + UGC brief)
- the supplier drafts in the 24 Nov procurement and legal reports
- the Nam Viet Gmail draft (read in Gmail, unsent)

Finance and inbox reports contain no other customer-facing drafts.

## Scorecard

| # | Item | Mark |
|---|---|---|
| 1 | D1_A_WhatsInIt.png | **PASS** |
| 2 | D2_B_PickYourPouch.png | **PASS** (note) |
| 3 | D3_B_BigSix.png | **PASS** |
| 4 | Script 1 "Fibre, minus the tub" | **FIX** (end card) |
| 5 | Script 2 "What's in my gym bag" | **FIX** (hook + end card) |
| 6 | Script 3 "The pile vs. the pouch" | **FIX** (replacement visual + end card) |
| 7 | UGC brief "My pre-launch first look" | **FIX** (mock-up pack lines) |
| 8 | Supplier follow-up template (procurement §3) | **PASS** |
| 9 | Ninie courtesy note (procurement §3) | **PASS** |
| 10 | Nam Viet Gmail draft (Peter + Ninie, unsent) | **FIX** (recipe offer before NDA) |
| 11 | Sand-M phone questions (procurement §6) | **PASS** |
| 12 | Supplier document request list (legal §3) | **PASS** |

**0 BLOCK.** No weight, GLP-1, therapeutic, before-and-after or competitor-name wording was found.

## 1. Today's ads (`gooday-launch/static-ads/daily/2026-11-24/`)

| Ad | Lines checked | Mark | Notes |
|---|---|---|---|
| D1_A_WhatsInIt | "What's in it. What's not." / "5 g collagen per pouch" / "made with Kakadu plum" / "<2 g sugar" / "~35 kcal" / ✗ Scoop ✗ Shaker ✗ Mixing / "Join the waitlist" | PASS | All Green. "What's not" lists only routine steps (scoop, shaker, mixing), not ingredients, so it implies no "free-from" or health claim. Kakadu wording carries no vitamin C claim. ~35 kcal matches product.md (target, covered by the small print) |
| D2_B_PickYourPouch | "Pick your pouch." / "Three flavours. 6 g fibre in each." / flavour chips | PASS | Green. Note: peach fibre and the grape colour are open decisions. If peach fibre is cut, the ad must change (ACL: don't show a range you won't sell). The pack band "Fibre + greens jelly" is the product name, not a "daily greens" claim |
| D3_B_BigSix | "6g of fibre in one squeeze-and-go pouch." / "About 25 kcal" / "Under 2 g sugar" / "No mixing, no shaker" | PASS | All Green. The large "6g" is a quantity, not a "good source" claim |

**All three:**
- The exact small print is present and legible.
- The pack's lower panel ("Good source of fibre", "Marine collagen peptides", "Tear, squeeze & go") is blurred and can't be read. I checked it at full size.
- The tiny "TEAR HERE" at the top of the pouch can't be read at feed size. Pack copy only; acceptable.
- No competitor is named or shown. The competitor patterns are layouts only.

## 2. Content set (`2026-11-24-content.md`)
The Content bot's own fixes (gut hook, #guthealth, recovery, glow, "replaces", "guilt-free") are confirmed. Three issues remain.

| Item | Mark | Problem | Exact fix |
|---|---|---|---|
| Scripts 1, 2, 3 end cards | FIX | The end cards show whole pouches and the outer bag. The lower panel ("Good source of fibre" = Amber; "Marine collagen peptides" = source undecided) and the bag's "ONE A DAY" can be read on a wide shot. Section 0's top-half rule covers close-ups only | Build the end cards from the soft-focused pack files (`static-ads/daily/2026-11-24/source/soften.py` makes `*_soft.png` versions of the round 3 pouches and bags), or crop to the top half. Live footage: keep the lower panel out of focus in every shot, wide ones too |
| Script 2 hook "What's in my gym bag (the new bit)" | FIX | First-person "my gym bag" with a mock-up implies someone already uses the product. Pre-launch, that reads as an implied testimonial (ACL s18/s29; claims.md open question on persona ads) | Change to: **"Packing the gym bag (coming soon)"**. Keep the caption "Gym bag, minus the shaker…" (PASS) |
| Script 3, 2 to 4 s "Hard cut: one green grape pouch where the pile was" + "…vs. the pouch" | FIX | The visual has the pouch replace the pile of capsules, the same issue as B5 "Swap the pile" (implies it replaces supplements; Red "Replaces your multivitamin") | Keep the pile in frame. Place the pouch **beside** it (no cut-away). On-screen text 0 to 4 s: **"Less to swallow than a pile of pills"** (exact Green line). Drop "…vs. the pouch". Beats 4 to 7 s then show just the pouch with "6 g fibre per pouch" |
| Scripts 1 to 3, all other lines and captions | PASS | | |
| UGC brief | FIX | Creators get printed mock-ups of the full round 3 pack, so an unboxing shows the bag's "Good source of fibre"/"Marine collagen peptides" and "ONE A DAY" lines and they can be read aloud | Before printing creator mock-ups, either (a) print with the lower line changed to **"6 g fibre per pouch"** (fibre) and **"Collagen peptides"** (collagen), and drop "ONE A DAY" on the bag, or (b) sticker over those lines. Add to "Please don't say or show": **"the small lines on the bottom half of the pack (they are placeholders)"**. Everything else PASS (Green list, disclosure, no taste or eating, 18+) |

## 3. Supplier and email drafts

| Item | Mark | Notes / exact fix |
|---|---|---|
| Follow-up template (due 27 Nov) | PASS | No claims, no pricing, konjac-free stated |
| Ninie courtesy note (procurement §3) | PASS | |
| **Nam Viet Gmail draft** (to Peter, cc Ninie, unsent) | FIX | Claims are fine (B2B spec, "about 7 g fibre" matches the RFQ). Two problems. First, "…or you need more detail on the recipe, just let me know and I'll send it through" offers the formula before an NDA, against the legal.md 24 Nov rule. Second, "Justin will confirm next steps" is in third person, but Justin signs the email. **Replace:** "If anything in the brief is unclear, just let me know." and "I'll confirm next steps once I've seen your answers." Justin edits the draft; the bot didn't change it |
| Sand-M call questions | PASS | |
| Supplier document list (legal §3) | PASS | |

## Marketing fix loop
No design got FIX, so no re-render was needed. **D1, D2 and D3 can go to Justin as PASS.**

## New questions for the consultant
None today. The persona/implied-testimonial question (22 Nov) also covers first-person "my bag" hooks.
