# Finance: unit economics v1

Finance bot, 23 Nov 2026 (status checked 24 Nov 2026). **No supplier has quoted yet**: 12 RFQs sent 23 Nov, 1 handover reply (see [suppliers.md](suppliers.md)), so nearly every cost here is **EST**. Facts with a source are linked. Assumptions: FX A$1 = US$0.65 = ฿23.5 (EST). "Unit" means one serve (one stick or one pouch). "Pack" means one bag of 28 (or 14). Mid-points are used where a range exists. Worked model: `../daily-bots/reports/2026-11-23-finance.md`.

## What this page says
1. **The 20 to 30 g stick is the money format.** The 28-pack weighs about 1 kg as sticks and about 3.8 kg as 120 g pouches. The pouch costs more to make and far more to post, and it never beats the stick.
2. **Best case: a Sand-M stick at A$59 for 28.** It lands at about A$0.36 a stick (EST), has an 80% gross margin and makes about A$27.70 contribution per order before ads (EST). Taiwan sticks make about A$19.60 (EST). NHP sticks make about A$10.30 (EST). The Taiwan pouch makes about A$2.50 (EST). The NHP pouch loses money at A$59.
3. **Ads decide everything.** The tracker's A$10 cost-per-signup target ([Settings tab](../gooday-launch/gooday-ad-test-tracker.xlsx)) gives a cost per first order of about A$67, if 15% of signups buy (EST). That is more than one order's contribution in every scenario, so Gooday needs subscribers who stay for 3 or more orders.
4. **Sea freight only, except for samples.** Air freight is about A$0.30 a stick and A$1.10 a pouch (EST). That cuts the Sand-M stick to about A$21 contribution and pushes every Asian pouch below zero.
5. **The first batch costs A$12k to A$41k (EST)** at the shortlisted MOQs. TCI's 200k MOQ needs about A$150k. For comparison, the lean launch budget is A$2.8k.

## 1. Landed cost per unit (EST unless linked)

| Per unit, A$ | Sand-M TH stick | Sand-M TH pouch | Taiwan stick | Taiwan pouch | NHP AU stick | NHP AU pouch |
|---|---|---|---|---|---|---|
| Ex-works jelly + fill | 0.24 | 0.38 | 0.50 | 0.75 | 0.85 | 1.10 |
| Printed film / spout pouch | 0.05 | 0.15 | 0.05 | 0.15 | 0.10 | 0.15 |
| Sea freight (LCL, incl. broker, port, biosecurity fees) | 0.07 | 0.12 | 0.07 | 0.12 | 0.03 road | 0.04 road |
| *Air freight instead* | *0.30* | *1.10* | *0.30* | *1.10* | n/a | n/a |
| AU import duty | **0%** (TAFTA)¹ | 0% | **5%** general rate² = 0.03 | 0.05 | none | none |
| **Landed (sea)** | **0.36** | **0.65** | **0.65** | **1.06** | **0.98** | **1.29** |

Basis: the Sand-M figure is ฿5 to 9 ex-works ([procurement report](../daily-bots/reports/2026-11-22-procurement.md); the Watsons shelf price of ฿20 and the Bangkok price of ฿102 for 4 support it). Taiwan is Wel-Bloom/TCI at A$0.40 to 0.70. NHP is A$0.90 to 1.60 a pouch, excluding formulation. The pouch fill is EST at 1.5x the stick (four times the mass of base jelly, the same actives). The collagen SKU adds about A$0.13 to 0.20 a unit (EST: ฿3 to 5 at Sand-M).
¹ Australia's tariffs on Thai-origin goods reached zero by 2015 ([DFAT TAFTA outcomes](https://www.dfat.gov.au/trade/agreements/in-force/tafta/Pages/key-outcomes-of-the-thailand-australia-free-trade-agreement)). This needs a TAFTA origin declaration. ² Taiwan has no FTA with Australia. 5% is EST for HS 2106.90 (food preparations), so check the HS code with a customs broker.

**GST.** Import GST is 10% of customs value + duty + freight. It is paid at the border and claimed back on the BAS, so it costs cash but not margin. On sales, this page **assumes the price includes 10% GST** (EST: the ATO treats confectionery and supplements as taxable, see [ATO taxable food](https://www.ato.gov.au/businesses-and-organisations/gst-excise-and-indirect-taxes/gst/in-detail/your-industry/gst-and-food/taxable-food); jelly isn't listed). A$59 incl. GST is A$53.64 net. If the product is GST-free, every order gains about A$5.40.

## 2. Per-order costs (EST unless linked)

| Per order | Stick pack | Pouch pack |
|---|---|---|
| Outer bag/box | 0.80 | 1.20 |
| 3PL pick and pack (A$2 to 5, [Eightx 3PL index](https://eightx.co/blog/australia-3pl-cost-index)) + mailer | 3.00 + 0.60 | 3.00 + 0.60 |
| Shipping, free to customer (28-pack about 1 kg vs 3.8 kg; 14-pack) | 10.00 (7.50) | 15.00 (10.00) |
| Shopify Payments, Basic: 1.75% + 30¢ domestic, 2.9% Amex, 3.5% intl ([Aspire](https://aspireapp.com/en-au/blog/shopify-fees-australia)); blended EST 2% + 30¢ | 1.48 at A$59 | 1.48 |
| Shopify Basic plan A$56/mo (A$42 annual) ([Aspire](https://aspireapp.com/en-au/blog/shopify-fees-australia)) | fixed cost | fixed cost |

## 3. Margin per order (sea freight, before ad cost; all EST)

Gross margin = (net revenue − units × landed − outer bag) / net revenue. Contribution = gross profit − 3PL − mailer − shipping − payment fees.

| Offer (incl. GST) | Sand-M stick | Sand-M pouch | Taiwan stick | Taiwan pouch | NHP stick | NHP pouch |
|---|---|---|---|---|---|---|
| **A$59 / 28** GM · contribution | **80% · A$27.68** | 64% · 14.16 | 65% · 19.63 | 42% · 2.54 | 47% · 10.32 | 30% · −3.76 |
| A$49 / 28 | 76% · 18.79 | 56% · 5.27 | 58% · 10.74 | 30% · −6.35 | 37% · 1.43 | 16% · −12.65 |
| A$69 / 28 | 83% · 36.57 | 69% · 23.05 | 70% · 28.52 | 51% · 11.43 | 55% · 19.21 | 41% · 5.13 |
| A$32 / 14 (price EST) | 80% · 11.21 | 65% · 4.25 | 66% · 7.19 | 45% · −1.56 | 50% · 2.53 | 34% · −4.71 |
| A$59 / 28, **air** | 68% · 21.24 | 13% · −13.28 | 53% · 13.19 | −9% · −24.90 | same as sea | same as sea |

A 14-pack keeps a similar gross margin, but shipping and pick fees halve its contribution. Use it as a trial pack, not as the core offer.

## 4. Ad cost (CAC) tied to the tracker

Tracker Settings (read 23 Nov 2026): target **A$10 per signup**, GO at 8%+ signup rate, STOP under 3%, pause an ad above 2x target (A$20). Daily log is empty, so there is no real CAC yet.

| A$59 / 28 stick | Sand-M | Taiwan | NHP |
|---|---|---|---|
| CAC per first order at A$10/signup and 15% signup-to-buyer (EST) | A$67 | A$67 | A$67 |
| Orders to pay back CAC | 2.4 | 3.4 | 6.5 |
| Highest cost per signup that pays back in 3 orders | A$12.50 | A$8.80 | A$4.60 |

So the A$10 target only works at Sand-M-like costs, or with better than 15% signup-to-buyer conversion. Update the tracker's target once real quotes land.

## 5. Break-even (contribution after fixed costs, ads counted separately)

| Monthly fixed cost (EST) | Sand-M stick | Taiwan stick | NHP stick | Sand-M pouch |
|---|---|---|---|---|
| A$500 (Shopify, apps, insurance, bookkeeping) | 18 orders | 26 | 49 | 35 |
| A$2,000 (plus always-on ads of about A$1.5k) | 72 | 102 | 194 | 141 |
| A$5,000 (plus agency or a part-time hire) | 181 | 255 | 485 | 353 |

One subscriber is about one 28-pack order a month.

## 6. First-batch cash (one SKU, sea freight; EST)

| Scenario | MOQ (EST unless published) | Landed stock | Import GST (refunded later) | Outer bags | R&D, samples | AU lab test | **Cash out** | Packs of 28 |
|---|---|---|---|---|---|---|---|---|
| Sand-M stick | 20k | 7,200 | 720 | 800 | 2,000 (no-konjac reformulation) | 1,500 | **≈ A$12k** | 714 |
| Sand-M pouch | 20k | 13,000 | 1,300 | 1,200 | 2,000 | 1,500 | ≈ A$19k | 714 |
| Wel-Bloom stick | 50k | 32,500 | 3,250 | 1,600 | 1,800 (US$200 fee published) | 1,500 | **≈ A$41k** | 1,785 |
| TCI stick | 200k (published) | 130,000 | 13,000 | 5,000 | 1,500 | 1,500 | ≈ A$150k | 7,140 |
| NHP stick | 10k | 9,800 | 980 (GST on invoice) | 800 | 10,000 (formulation) | 1,500 | **≈ A$23k** | 357 |

Both SKUs roughly double the cash (Sand-M stick about A$23k). Factories often take a 30 to 50% deposit (EST).

## 7. Launch budget vs spend

Totals are from the Notion [ad test launch pack](https://app.notion.com/p/41514ab463ca813fa928ca820f143ae9) (estimates, not quotes). The line split is Finance bot EST.

| Item | Lean A$ | Comfortable A$ | Spent so far |
|---|---|---|---|
| Meta ad test (8 ads × A$10 × 7 days; a second wave if comfortable) | 560 | 1,500 | unknown / 0 |
| Domain, handles, Shopify (3 or 6 months) | 220 | 400 | unknown / 0 |
| Regulatory consultant | 1,000 | 2,500 | 0 |
| Supplier samples + courier | 450 | 1,200 | 0 |
| AU lab tests (micro, nutrition panel) | 0 | 2,000 | 0 |
| Trade mark (1 or 2 classes) | 400 | 800 | 0 |
| Creator gifting / paid posts | 0 | 800 | 0 |
| Mock-ups, print proofs | 200 | 200 | unknown / 0 |
| **Total** | **2,830 (≈2.8k)** | **9,400** | **unknown / 0** |

Neither budget covers a first production batch (section 6).

## Firm these up first
1. **Ex-works price per stick at 20k/50k units**, ask Sand-M and Wel-Bloom. This moves margin more than anything else.
2. **Real cost per signup and signup-to-buyer rate** from the ad test (Daily log is still empty).
3. **GST status of a functional jelly** (ATO ruling or accountant) and the **HS code / duty for Taiwan**.

Open question for founders (not decided): the format numbers point strongly to the stick. See [decisions.md](decisions.md).

## 8. What the RFQ replies will change (24 Nov 2026)
Detail: `../daily-bots/reports/2026-11-24-finance.md`.
- **Unit price tiers (RFQ q4)** replace section 1 "Ex-works jelly + fill". The biggest lever: every A$0.10 a stick moves contribution by about A$2.80 per 28-pack order (EST); A$0.25 a pouch moves it by A$7.00.
- **MOQ and printed-film MOQ (q3)** replace section 6. Film MOQ can be higher than the jelly MOQ and set the real minimum batch.
- **Sample price and shipping (q2)** replace the section 7 samples line.
- **Lead time (q5)** and deposit terms set cash timing (deposit EST 30 to 50%), not margin.
- **Supplier country** sets duty: Taiwan 5% (EST, no FTA); China, Korea, Japan, Vietnam, Malaysia and Thailand have FTAs with Australia, so 0% is likely (EST; needs a certificate of origin; broker to confirm HS code).
- **Who supplies ingredients (q6)** and bovine vs marine price change the collagen adder (A$0.13 to 0.20 a unit, EST).
- Once a written quote lands, the matching cells here change from EST to "quote, <date>".

## 9. Sample budget EST (about 5 suppliers, both SKUs, to Melbourne; 24 Nov 2026)
| Per supplier | Low | Mid | High |
|---|---|---|---|
| Sample fee (Wel-Bloom US$200 refundable is published; others EST) | US$0 | US$80 | US$200 |
| Express courier, 1 to 2 kg (EST) | US$35 | US$60 | US$110 |
| **× 5 suppliers** | **≈ A$270** | **≈ A$1,080** | **≈ A$2,385** |
| Border contingency for collagen/gelatin samples (permit, broker; EST) | A$0 | A$300 | A$800 |
| **Total EST** | **≈ A$270** | **≈ A$1,380** | **≈ A$3,185** |

Duty and import GST EST A$0 if each consignment stays under A$1,000. Not included: AU lab screen before tasting (EST A$150 to 300 a sample; test the 2 or 3 finalists only) and stage-2 custom prototypes (R&D EST US$0 to 500 each, top 2 only). The mid case sits near the "comfortable" A$1,200 samples line in section 7 and well above the "lean" A$450. Suggested (Justin decides): stock samples first, courier quote in writing before paying anything, collagen samples only from finalists.
