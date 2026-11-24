# Formulation: benchmark, doses, recommended formula

Nutritionist bot, 23 Nov 2026. **This is a proposal. Justin decides** (open item in [decisions.md](decisions.md)). It is general information, not medical advice. Facts are dated and linked. EST means an estimate (no supplier quote or lab result yet). FX EST: A$1 = US$0.65 = ฿23.5 = CA$0.91. All web sources were checked on 23 Nov 2026. Safety review by ingredient (who should avoid, drug timing): `../daily-bots/reports/2026-11-22-nutritionist.md`. Summary report: `../daily-bots/reports/2026-11-23-nutritionist.md`.

## The answer in brief

| Per serve (label value) | **Fibre + greens, green apple** | **Collagen + Kakadu plum, peach** |
|---|---|---|
| Hero | **7 g fibre** (design 7.7 g): 4.5 g resistant dextrin + 2.5 g acacia + 1.0 g PHGG + pectin gel | **6 g bovine collagen peptides = about 5.4 g protein** |
| Extras | 1.0 g greens (stick) / 1.5 g (pouch): spinach, kale, broccoli, spirulina. No wheatgrass. | Kakadu plum 0.25 g + acerola 0.15 g, about 45 mg vitamin C at fill. Claim **10 mg (25% RDI)** until stability data exist |
| Gel | Amidated LM apple pectin + calcium (or gellan) | Gellan (high-acyl + low-acyl). Gelatin is the fallback |
| Sweetener | Stevia Reb M + monk fruit. **No erythritol, no sucralose** | Same |
| kcal / sugar | about 21 kcal / <1 g (stick); 26 kcal / <2 g (pouch) | about 27 kcal / <1 g (stick); 32 kcal / <2 g (pouch) |
| FSANZ claims it unlocks (Compliance + consultant to confirm) | "**Excellent source of fibre**" (≥7 g); "fibre contributes to regular laxation" | "**Source of protein**" (≥5 g); "**good source of vitamin C**" (≥25% RDI); "vitamin C **contributes to normal collagen formation for the normal function of skin**" |
| Ingredient cost (EST) | A$0.15 stick / A$0.17 pouch | A$0.22 stick / A$0.24 pouch |

The same actives work in both formats. The 30 g stick is denser, so its gel and texture risk is higher. See [finance.md](finance.md) for why the stick is the money format.

## 1. Benchmark: what brands put in one serve (checked 23 Nov 2026)

### Fibre and greens

| Product | Format / serve | Fibre per serve and type | Greens / other actives | Sweetener | Gel | kcal | Sugar | Price per serve (local → A$ EST) | Source |
|---|---|---|---|---|---|---|---|---|---|
| Grüns Superfood Gummies | 8 gummies (pack) | 6 g: tapioca fibre (FiberSMART) + inulin | 60+ greens/fruit (amounts undisclosed); 21 added vitamins and minerals | Cane sugar; sugar-free version uses allulose + Reb M | Pectin | 50 (20 SF) | 8 g (<1 g SF) | US$1.07 sub / $2.38 one-off → A$1.65 / 3.66 | [Medical News Today](https://www.medicalnewstoday.com/articles/gruns-gummies-review), [gruns.co](https://gruns.co/) |
| AG1 | 12 g powder scoop | 2 g (blend) | Proprietary greens blends (no mg given); probiotics; full-DV vitamin C (added) | Stevia | n/a | 50 | <1 g (EST) | US$2.48 to 3.30 → A$3.80 to 5.10 | [Torokhtiy review](https://torokhtiy.com/blogs/review/ag1-review) |
| Bloom Greens & Superfoods | 1 scoop (~5.7 g) | 2 g: chicory FOS, flaxseed, apple powder, agave inulin | Greens blends (no mg); added vit C 90 mg, B12, D, chromium 200 mcg | Stevia | n/a | 15 | "no added" | US$1.00 → A$1.54 | [H-E-B listing](https://www.heb.com/product-detail/12347046) |
| Benefiber (AU) On the Go | 3.5 g stick | 3 g wheat dextrin (only ingredient) | none | none | n/a | 8 | <1 g | A$7.10 / 28 sale (RRP A$12.99) → A$0.25 to 0.46 | [Discount Chemist](https://discountchemist.com.au/benefiber-on-the-go-28-sticks/) |
| Metamucil Fiber Gummies, no sugar added | 3 gummies | 5 g: inulin + soluble corn fibre (not psyllium) | none | Xylitol (polyol) | Pectin | 0 (listed) | 0 g | Price not listed; EST US$0.60 → A$0.95 | [Stop & Shop](https://stopandshop.com/groceries/health-beauty/digestive-health-nausea/fiber/metamucil-no-sugar-added-orange-flavored-fiber-gummies-72-ct-btl.html) |
| Physician's Choice Fiber Gummies | 2 gummies | 5 g chicory root (inulin) | none | "no added sugar or artificial sweeteners" (not named) | Pectin | 15 | <1 g | US$0.70 → A$1.08 | [GNC](https://www.gnc.com/fiber/620453.html) |
| **Physician's Choice Fiber Jelly** (US, launched Oct 2026) | squeeze stick (size not published) | 6 g "prebiotic fibre" (type not published) | **600 mcg chromium picolinate** (not allowed as an added mineral in an AU food) | Not published | Not published | 30 | <1 g | Not published (waitlist, 40% off first box) | [physicianschoice.com](https://physicianschoice.com/pages/fiber-jelly), [Nutraceuticals World](https://www.nutraceuticalsworld.com/breaking-news/physicians-choice-launches-fiber-jelly/) |
| **Jelly Me Cuti Activ Fiber** (Sand-M, TH) | 30 g stick | 7 g, mostly acacia (≈6.8 g of a 90% fibre ingredient) | apple and blackcurrant extracts | Sucralose + acesulfame K | **Konjac + carrageenan + LBG** (banned route for Gooday) | low (illegible) | 0 g | ฿20 → A$0.85 | [Watsons TH](https://www.watsons.co.th/en/handy-herb-handy-herb-jelly-me-cuti-fiber-30g./p/BP_318844), [procurement report](../daily-bots/reports/2026-11-22-procurement.md) |
| **Goli Gut Stik** (US, 12 Nov 2026) | 25 g jelly stick | **1.7 g**: 1 g chicory root + 0.7 g XOS; heat-treated B. longum | none | not stated | not stated | 25 to 30 | ~half of 7 to 9 g carbs | US$2.50 → A$3.84 | [Stack3d](https://www.stack3d.com/2026/11/goli-nutrition-stik-series/) (24 Nov) |
| Olipop (prebiotic soda) | 355 mL can | 9 g: cassava fibre + chicory and Jerusalem artichoke inulin | botanical extracts | Stevia + cassava syrup + juice | n/a | 45 | 4 g | US$2.28 → A$3.51 | [H-E-B Olipop](https://www.heb.com/product-detail/olipop-tropical-punch-9g-fiber-prebiotic-soda/6637501) |

### Collagen

| Product | Format / serve | Collagen type and dose | Vitamin C and source | Other actives | Sweetener | Gel | kcal | Sugar | Price per serve (→ A$ EST) | Source |
|---|---|---|---|---|---|---|---|---|---|---|
| Vital Proteins Collagen Peptides | 20 g powder | **20 g bovine** (18 g protein) | none on this listing | none | none | n/a | 70 | 0 | US$1.68 → A$2.58 | [Vitacost](https://www.vitacost.com/products/vital-proteins-collagen-peptides-unflavored-20-oz-567-g-71356) |
| **Jelly Me Cuti Multi Collagen** (Sand-M, TH) | 30 g stick | **2 g fish** collagen peptide (3 g protein) | 60% Thai RDI (source not stated) | **6 g fibre** | not recorded | Konjac + carrageenan + LBG | 35 | 0 | 4 for ฿102 → A$1.09 | [procurement report](../daily-bots/reports/2026-11-22-procurement.md) (pack photos) |
| Everydaze Essential Collagen Solution (KR) | 20 g stick | **"plant-based collagen (hibiscus)"**, not real collagen; "3,000 mg" on Target | 0 mg | FOS | Erythritol + stevia | LBG, xanthan, agar, tamarind | 30 | 2 g | US$1.50 → A$2.31 | [Vitacost](https://www.vitacost.com/products/everydaze-essential-collagen-solution-jelly-stick-peach-10-sticks-0-7-oz-20-g-each-121681), [Target](https://www.target.com/p/everydaze-essential-collagen-solution-jelly-stick-peach/-/A-1002316290) |
| grn+ Volume Up Collagen Jelly (KR) | 15 g stick | low-MW fish (tilapia) collagen, mg not stated | added (mg not stated) | elastin, HA, glutathione, FOS | Stevia | LBG, xanthan, tamarind | 24 | n/s | US$1.83 → A$2.81 | [Dodoskin](https://www.dodoskin.com/collections/grn/products/grn-volume-up-collagen-jelly-15g-14ea) |
| Earth Pharmaceutical Collagen C Jelly (JP) | 10 g stick | **~2.5 g fish** collagen | up to ~25 mg (added) | shark/salmon cartilage, glucosamine | Erythritol + ace-K + sucralose | "polysaccharide thickener" | ~12 | ~0.5 g carb | CA$2.27 → A$2.50 | [Yami](https://www.yami.com/ca/en/p/collagen-c-jelly-peach-flavor-10g-34-packets-individually-wrapped/3174109171) |
| FANCL Collagen Jelly (JP) | 20 g stick | **3 g** collagen peptides | n/s | HA, ceramide, rosebud | n/s | n/s | n/s | n/s | US$2.20 → A$3.38 | [Weee](https://www.weee.com/en/product/FANCL-Collagen-Jelly-Bar-20g-x-10-Bars/2866264) |
| Swisse Collagen Peptides Gummies (AU) | 3 gummies | **Verisol B (bovine), 27.8% of gummy**; about 2.5 g (EST from %) | acerola (mg not stated) | none | Maltitol, sorbitol, stevia | Bovine gelatine | n/s | "99% sugar free" | A$29.99 / 15 serves → A$2.00 | [swisse.com.au](https://swisse.com.au/products/swisse-collagen-peptides-gummies) |
| Nature's Way High Strength Collagen Vita Gummies (AU) | 2 pastilles | "2,500 mg" hydrolysed collagen (page also says 1.25 g: conflict) | not stated | vit E, zinc | Sucralose, maltitol, sorbitol | n/s | n/s | sugar free | A$18.99 / 25 → A$0.76 (sale) | [Chemist Warehouse](https://www.chemistwarehouse.com.au/buy/117601/nature-s-way-adult-vita-gummies-sugar-free-high-strength-collagen-50-gummies) |
| **WELLINUS Collagen jelly stick** (KR, The Honest Farmer) | stick (~25 g EST) | low-MW **marine (cod)** collagen; mg not published in English listings | n/s | 60M+ sticks sold (company); OEM/ODM factory | n/s ('no added sugar') | n/s | n/s | n/s | US$2.72 → A$4.18 (US reseller) | [PR Newswire Asia](https://en.prnasia.com/releases/global/the-honest-farmer-co-ltd-s-wellinus-collagen-jelly-sticks-surpass-60-million-sticks-sold-in-korea-follow-up-products-in-development-557623.shtml), [Underyours](https://underyours.com/products/wellinus-collagen-full-of-mango-jelly-stick-marine-collagen-fast-absorbing-snack-ultra-low-weight-molecular-marine-collagen-haccp-certified-22-05-oz-pack-of-25) (24 Nov) |
| Morinaga Oishii Collagen Drink (JP) | 125 mL carton | **10 g** collagen peptide (incl. pork), 10 g protein | added (mg n/s) | none | Sugar + stevia + monk fruit | n/a | 72 | ≤8 g carb | US$3.68 → A$5.65 | [Japanese Taste](https://int.japanesetaste.com/products/morinaga-oishi-collagen-drink-peach-flavor-12-cartons) |

**What the benchmark shows**
1. Fibre gummies and jellies cluster at **5 to 6 g**, and most use **inulin or chicory**, which are high-FODMAP and gassy. Only Jelly Me reaches 7 g, and it uses acacia in a konjac gel.
2. Collagen jelly sticks carry only **2 to 3 g** of collagen, and some carry plant "collagen" that is not collagen at all. The only 10 g products are powders and drinks.
3. Most competitors rely on **added vitamins** (AG1, Bloom, Grüns) or **polyols and artificial sweeteners** (erythritol, maltitol, sucralose, ace-K, xylitol). Gooday can do neither in Australia without problems, and doesn't need to.

## 2. Effective doses from the evidence

| Ingredient | Dose used in RCTs / meta-analyses | GI tolerance | Fit for a 30 g jelly | Links |
|---|---|---|---|---|
| Resistant dextrin (Nutriose, Fibersol) | 8 to 30 g/day for weight, glucose and lipids (small, low to moderate certainty effects) | Very well tolerated. Long-term trials ran to about 45 g/day | **Yes**: low viscosity, neutral taste, cheap | [PMC5434557](https://pmc.ncbi.nlm.nih.gov/articles/PMC5434557/), [BMC Nutr 2025](https://link.springer.com/10.1186/s40795-025-01080-8), [Roquette tolerance poster](https://www.roquette.com/-/media/roquette-sharepoint-libraries/marcomonline---food-and-nutrition/roquette-food-spec-nutrition-poster-2006-helsinki-nutriose-prebiotic-effect.pdf) |
| Soluble corn fibre (Promitor) | 10 to 20 g/day raised faecal weight | Similar corn-starch fibre: mild symptoms from about 30 g single dose | Yes (alternative to dextrin) | [PubMed 23427334](https://pubmed.ncbi.nlm.nih.gov/23427334/), [PubMed 27346078](https://pubmed.ncbi.nlm.nih.gov/27346078/) |
| Acacia gum (gum arabic) | Prebiotic effect 5 to 40 g/day; **10 g/day optimal** | High tolerance; slow fermentation, less gas than inulin | **Yes**: low viscosity, proven in Jelly Me at 7 g | [Calame 2008, Br J Nutr](https://www.doi.org/10.1017/S0007114508981447), [NutraIngredients](https://nutraingredients.com/Article/2008/11/20/Gum-arabic-shows-prebiotic-potential-in-humans-Study) |
| Partially hydrolysed guar gum (Sunfiber) | **About 5 to 6 g/day** in constipation and IBS trials | Well tolerated; certified low-FODMAP product exists (check certificate) | **Yes**: low viscosity, neutral. Costs more | [PubMed 24711073](https://pubmed.ncbi.nlm.nih.gov/24711073/), [IBS RCT PMC4744437](https://pmc.ncbi.nlm.nih.gov/articles/PMC4744437), [PHGG meta-analysis](https://doaj.org/article/a0c960648a9046e69ce125917697fafe) |
| Psyllium | About 10 g/day lowers LDL; also the best constipation evidence | Good, but it swells | **No**: forms a thick gel, gritty, sets in the pack | [Jovanovski 2018, PubMed 30239559](https://pubmed.ncbi.nlm.nih.gov/30239559/) |
| Oat beta-glucan | **3 g/day** lowers LDL (FSANZ high-level claim exists) | Good | **No for now**: very viscous and costly at 3 g. Future SKU idea | [Ho 2016, PubMed 27724985](https://pubmed.ncbi.nlm.nih.gov/27724985/) |
| Inulin / FOS | 5 to 20 g/day; short-chain fructans raised stool frequency | Gas and bloating rise with dose, often from 5 to 10 g. **High FODMAP** | Avoid as the hero fibre | [β-fructan meta-analysis](https://mdpi.com/2072-6643/11/1/91/htm) |
| Apple pectin | **15 g/day** lowered LDL in an RCT (pectin type mattered) | Good | Gel only (0.4 to 0.7 g); no health effect at this dose | [Brouns 2012, PubMed 22190137](https://pubmed.ncbi.nlm.nih.gov/22190137/) |
| Greens powders | **No robust RCTs**. Trials used 10 g+ proprietary blends | Fine; heavy-metal and gluten risk | 1 to 2 g is under a quarter of a vegetable serve. **Taste, colour and story only** | [2026-11-22 review](../daily-bots/reports/2026-11-22-nutritionist.md) |
| Hydrolysed collagen peptides | Skin 2.5 to 10 g/day (Verisol 2.5 g); joints about 10 g/day. Independent, high-quality trials show no clear skin effect | Very well tolerated | **Yes** to about 6 g in a stick; 10 g needs the pouch | [Proksch 2014, PubMed 24401291](https://pubmed.ncbi.nlm.nih.gov/24401291/), [Pu 2023, PubMed 37432180](https://pubmed.ncbi.nlm.nih.gov/37432180/), [2025 meta PubMed 40761858](https://pubmed.ncbi.nlm.nih.gov/40761858/) |
| Vitamin C: Kakadu plum / acerola | AU label RDI 40 mg. Claim needs ≥10% RDI (4 mg); "good source" ≥25% (10 mg). Kakadu fruit 2,300 to 3,150 mg/100 g fresh (about 14% dry); freeze-dried powder about 8,300 mg/100 g (company test). Acerola powders are sold at 17% vitamin C | No GI issue at food doses; stones risk only near 1,000 mg/day | **Yes**. Heat and oxygen destroy it, so claim the end-of-shelf-life value | [Molecules 2023](https://www.mdpi.com/1420-3049/28/6/2828), [Aust. Superfood Co.](https://austsuperfoods.com.au/the-vitamin-c-powerhouse-kakadu-plum), [Givaudan Acerola 17%](https://knowde.com/stores/givaudan-naturex/products/acerolife-17-vitamin-c-naturally-occuring-en849304) |
| Stevia (steviol glycosides, Reb M) | ADI 4 mg/kg/day (steviol equivalents); a serve uses about 12 to 35 mg | None | Yes. Reb M is the least bitter grade | [FSANZ sweeteners](https://www.foodstandards.gov.au/consumer/additives/sweeteners) |
| Monk fruit (luo han guo extract) | Permitted as a food additive in AU/NZ (FSANZ A1129, 2019) | None | Yes, at 5 to 20 mg to round off stevia | [FSANZ A1129 approval](https://mta-sts.foodstandards.gov.au/sites/default/files/food-standards-code/applications/Documents/A1129%20Approval%20report.pdf) |
| Allulose | Approved novel food (A1247, 2024). **Excluded from "sugars"** on the NIP; energy 2 kJ/g | Laxative above about 0.4 g/kg single dose. **Requires a "may have a laxative effect" statement** in confectionery and dessert classes; use limits by class | Optional taste fix (1 to 2 g) only. The laxative statement is a poor fit for a gut brand | [A1247 approval report](https://foodstandards.gov.au/sites/default/files/2024-08/A1247%20Approval%20Report.pdf) |
| Erythritol | GI effects above about 0.5 g/kg; it stacks with fibre | Cardiovascular platelet signal (observational, plus a 30 g challenge) | **Not used.** Unresolved safety signal and a stacking GI load, for no benefit that stevia + monk fruit can't give | [Witkowski 2023, PMC10275890](https://pmc.ncbi.nlm.nih.gov/articles/PMC10275890/) |

FSANZ thresholds (Schedule 4, read 23 Nov 2026, [legislation.gov.au](https://www.legislation.gov.au/F2015L00474/2024-10-29/2024-10-29/text/original/epub/OEBPS/document_1/document_1.html)): fibre ≥2 g "source", ≥4 g "good source", ≥7 g "excellent source"; protein ≥5 g "source", ≥10 g "good source"; a vitamin claim needs ≥10% RDI, and "good source" needs ≥25%. Permitted general-level health claims include fibre "contributes to regular laxation", and vitamin C "contributes to normal collagen formation for the normal function of skin" (also cartilage and bones, teeth and gums). Every health claim also needs the food to pass the Nutrient Profiling Scoring Criterion (NPSC).

## 3. Recommended formula (proposal)

Daily targets used: fibre 30 g (NIP reference; women's AI 25 g), protein 50 g, vitamin C 40 mg RDI. Energy factors: fibre 8 kJ/g, protein and sugar 17 kJ/g. All composition figures are EST until a lab tests the samples.

### 3a. Fibre + greens, green apple

| Ingredient (per serve) | **30 g stick** | % w/w | **120 g pouch** | % w/w | Why |
|---|---|---|---|---|---|
| Resistant dextrin (Fibersol-2 or Nutriose, ~90% fibre) | 4.50 g | 15.0 | 4.50 g | 3.8 | Base fibre: cheap, neutral, low viscosity, best tolerated |
| Acacia gum (Fibregum-type, ~90% fibre) | 2.50 g | 8.3 | 2.50 g | 2.1 | Slow fermentation, less gas; proven in a 7 g jelly stick |
| PHGG (Sunfiber-type, ~85% fibre) | 1.00 g | 3.3 | 1.00 g | 0.8 | Gut-comfort evidence; low-FODMAP route |
| Greens blend: spinach 40%, kale 30%, broccoli 20%, spirulina 10% (steam-treated, low micro) | 1.00 g | 3.3 | 1.50 g | 1.3 | Taste, colour and story. Print the grams. No wheatgrass (gluten cross-contact) |
| Green apple juice concentrate (65 °Brix) | 0.80 g | 2.7 | 2.00 g | 1.7 | Real fruit taste; holds sugar under 1 g / 2 g |
| Amidated LM apple pectin | 0.39 g | **1.3** | 0.72 g | **0.6** | Vegan gel at low sugar (HM pectin needs sugar) |
| Calcium lactate | 0.03 g | 0.1 | 0.06 g | 0.05 | Sets the LM pectin |
| *Alt. gel: gellan high-acyl + low-acyl* | *0.045 + 0.015 g* | *0.15 + 0.05* | *0.10 + 0.04 g* | *0.08 + 0.03* | Use if the pectin gel weeps or is too weak |
| Malic acid / citric acid / sodium citrate (target pH 3.5 ± 0.1) | 0.12 / 0.06 / 0.03 g | 0.7 total | 0.36 / 0.12 / 0.06 g | 0.45 total | Green apple sourness, gel set, microbial safety |
| Natural green apple flavour | 0.12 g | 0.4 | 0.42 g | 0.35 | Masks acacia and greens notes |
| Steviol glycosides (Reb M) + monk fruit extract (MV 50%) | 12 mg + 6 mg | 0.06 | 30 mg + 15 mg | 0.04 | Sweet with no sugar, polyol or bitterness |
| Preservative | none if hot-fill (≥85 °C) at pH ≤3.8 is validated; otherwise potassium sorbate at the permitted level (factory confirms) | | same | | Clean label |
| Water | to 30 g (≈19.4 g) | | to 120 g (≈106.7 g) | | |

| Result per serve (EST) | Stick | Pouch | % daily target |
|---|---|---|---|
| Dietary fibre | 7.7 g designed, **label 7.0 g** | 8.2 g designed, **label 7.0 g** | 23% of 30 g (28% of women's 25 g) |
| Sugars | ~0.7 g (label <1 g) | ~1.5 g (label <2 g) | |
| Energy | ~86 kJ / **21 kcal** | ~110 kJ / **26 kcal** | ~1% |
| Protein | ~0.3 g | ~0.5 g | |
| Claims (Compliance + consultant) | "Excellent source of fibre"; "7 g fibre"; "fibre contributes to regular laxation" (NPSC must pass) | Same | |
| Ingredient cost EST | **A$0.15** | **A$0.17** | |

**Good / better / best (fibre)**

| Option | Fibre system | Label fibre | Claim | Cost EST (stick) | Trade-off |
|---|---|---|---|---|---|
| Good | 6.5 g resistant dextrin + pectin | 6 g | "Good source of fibre" | A$0.12 | Cheapest and simplest gel trial. Same as the old spec, and no better than Physician's Choice |
| **Better (recommended)** | 4.5 g RD + 2.5 g acacia + 1.0 g PHGG + pectin | **7 g** | **"Excellent source"** | **A$0.15** | Beats every 5 to 6 g gummy and jelly. Three gentle fibres spread the fermentation |
| Best | 5.0 g PHGG + 2.5 g acacia + 0.5 g RD + pectin | 7 g | Excellent source, plus a Monash low-FODMAP certification route | A$0.20 + certification fee | PHGG at its trial dose: the strongest "gentle on the gut" story. PHGG supply and price are concentrated in one supplier |

**Why this beats competitors:** it has more fibre than Grüns, Metamucil and Physician's Choice gummies (5 to 6 g) and matches Jelly Me at 7 g. It uses no inulin or chicory (the gas complaint Physician's Choice itself advertises against: [landing page](https://physicianschoice.com/pages/fiber-gummies-v4)), no polyols, no added vitamins and no konjac. It is about 21 kcal versus Grüns at 50.

### 3b. Collagen + Kakadu plum, peach

| Ingredient (per serve) | **30 g stick** | % w/w | **120 g pouch** | % w/w | Why |
|---|---|---|---|---|---|
| Hydrolysed **bovine** collagen peptides (2 to 5 kDa, low-odour grade, halal-certified, BSE-free documents) | **6.00 g** | 20.0 | **6.00 g** | 5.0 | ≥5 g protein with margin. No fish allergen; halal possible; cheaper and less odour than marine |
| Kakadu plum, freeze-dried powder (≈8,300 mg vit C/100 g, EST) | 0.25 g | 0.8 | 0.25 g | 0.2 | ≈21 mg vitamin C; Australian native hero |
| Acerola juice powder, 17% **naturally occurring** vitamin C (CoA: no added ascorbic acid) | 0.15 g | 0.5 | 0.15 g | 0.13 | ≈25 mg vitamin C, cheaply. Total ≈46 mg at fill |
| Peach juice concentrate (65 °Brix) | 1.20 g | 4.0 | 2.50 g | 2.1 | Peach body; covers the brothy collagen note |
| Gellan, high-acyl + low-acyl | 0.045 + 0.015 g | **0.15 + 0.05** | 0.10 + 0.04 g | **0.08 + 0.03** | Soft, squeezable, heat-stable gel; less haze with peptides than pectin (trial) |
| *Fallback gel: bovine gelatin 250 bloom* | *0.6 g* | *2.0* | *1.8 g* | *1.5* | Fully protein-compatible. It melts around 30 °C, so it turns to liquid in an Aussie summer (it still drinks) |
| Calcium lactate | 0.015 g | 0.05 | 0.04 g | 0.03 | Gellan set |
| Citric / malic acid / sodium citrate (target pH 3.6 ± 0.1) | 0.15 / 0.06 / 0.03 g | 0.8 total | 0.48 / 0.12 / 0.12 g | 0.6 total | Collagen buffers acid, so it needs more acid than the fibre SKU |
| Natural peach flavour (+ a touch of vanilla) | 0.15 g | 0.5 | 0.48 g | 0.4 | Masks peptide bitterness |
| Steviol glycosides (Reb M) + monk fruit extract | 12 mg + 6 mg | 0.06 | 35 mg + 18 mg | 0.04 | As for fibre |
| Preservative | as for fibre | | | | |
| Water | to 30 g (≈21.9 g) | | to 120 g (≈109.7 g) | | |

| Result per serve (EST) | Stick | Pouch | % daily target |
|---|---|---|---|
| Collagen / protein | 6 g / **≈5.4 g protein** (lab to confirm the nitrogen factor) | same | 11% of 50 g |
| Vitamin C | ≈46 mg at fill; EST 18 to 28 mg at 12 months; **claim 10 mg** until stability data | lower retention likely (spout lets in oxygen) | Claim 25% RDI; likely 45 to 70% |
| Sugars | ~0.9 g (label <1 g) | ~1.8 g (label <2 g) | |
| Energy | ~113 kJ / **27 kcal** | ~134 kJ / **32 kcal** | ~1.5% |
| Claims (Compliance + consultant) | "Source of protein"; "good source of vitamin C"; "vitamin C contributes to normal collagen formation for the normal function of skin" (NPSC must pass). Still no claim for collagen itself | same | |
| Ingredient cost EST | **A$0.22** | **A$0.24** | |

**Good / better / best (collagen)**

| Option | Formula change | Protein | Claims | Cost EST | Trade-off |
|---|---|---|---|---|---|
| Good | 5 g generic collagen; acerola 0.25 g + Kakadu 0.1 g | ~4.5 g | Vitamin C claims only ("source of protein" fails) | A$0.15 | A tiny Kakadu share risks a misleading "vitamin C from Kakadu" story (ACL) |
| **Better (recommended)** | 6 g bovine peptides; Kakadu 0.25 g + acerola 0.15 g | **5.4 g** | **Source of protein + good source of vitamin C + collagen-formation-for-skin (vit C)** | **A$0.22 stick** | Best claim set per dollar; 2 to 3 times the collagen of Jelly Me, FANCL and the Earth sticks |
| Best (pouch; or a 40 g stick) | 10.5 g peptides (incl. **2.5 g Verisol B**, the studied skin dose) + 2.5 g acacia; vitamin C from **Kakadu only (0.5 g)** | ≈9.5 to 10 g (needs ≥10 g) | Adds "good source of protein" if ≥10 g, "source of fibre" (≥2 g), and "vitamin C from Kakadu plum" cleanly | A$0.55 to 0.65 | 10 g matches joint-trial doses and Morinaga. Too dense for a 30 g stick (35% w/w); more cost and kcal (≈45) |

**Why this beats competitors:** it has real animal collagen at 6 g, versus 2 to 3 g in the Asian sticks and "hibiscus collagen" in Everydaze. Its vitamin C comes from food (Kakadu plum + acerola) and is high enough to unlock the one permitted skin-related claim, which comes through vitamin C. It uses no polyols or artificial sweeteners (unlike Swisse, Nature's Way and Earth), and it is bovine, so it is fish-free and halal-possible.

## 4. Risks: taste, texture and gel
1. **The no-konjac gel at high solids is the biggest technical risk.** Fibre solids are about 28% w/w in the stick. LM pectin may weep (syneresis) or set too firm, and gellan may break into lumps when squeezed. Run a texture and syneresis trial at 4, 25, 30 and 40 °C over 12 weeks.
2. **Collagen with anionic gels.** At pH 3.4 to 3.8, collagen peptides carry a positive charge and can complex with pectin or gellan. That causes haze, grain or a weaker gel. Use low-MW peptides, add them after the gel is hydrated, and trial gellan versus pectin versus gelatin side by side.
3. **Greens colour and taste.** At low pH and with heat, chlorophyll turns olive-brown, and spirulina blue fades. Use an opaque film, and accept a yellow-green or use copper chlorophyllin only if Justin accepts an added colour. Greens also bring a grassy bitterness. Green apple and malic acid mask it, and keeping greens at 1 to 1.5 g limits it.
4. **Bitterness and off-notes.** Collagen gives a brothy or bitter note. Acacia can add a woody note. Reb M can leave a lingering taste above about 15 mg in 30 g. Adjust with flavour and acid before adding more sweetener.
5. **Browning and vitamin C loss.** Peptides plus reducing sugars plus ascorbate can brown (Maillard) over 12 months. Keep juice low, use a high-barrier foil film, and nitrogen-flush the pouch.
6. **GI comfort.** 7 g of mixed fibre is mild for most people. Pack advice: "start with one a day, drink water". Space from medicines by 2 hours (see the safety review).

## 5. What the factory and lab must confirm (before any claim)
1. In writing: **no konjac, glucomannan or carrageenan**, including line cross-contact.
2. A gel trial at these loads, with squeeze force through the stick or spout, plus syneresis and texture at 12 weeks.
3. A hot-fill or pasteurisation validation (≥85 °C), pH ≤3.8, °Brix and water activity, with a micro challenge test. Decide whether a preservative is needed.
4. **Fibre measured by AOAC 2009.01 or 2011.25** at an AU lab. Older methods miss resistant dextrin and would under-read the 7 g.
5. **Protein** by Kjeldahl or Dumas, with the nitrogen factor stated. It must be ≥5.0 g at release.
6. A **vitamin C stability study** (HPLC at 0, 3, 6 and 12 months) to set the claim and the Kakadu amount. The consultant decides whether overage counts as "added" (open in [claims.md](claims.md)).
7. Raw material CoAs: heavy metals (greens, Kakadu, collagen), pesticides, gluten (greens), halal and BSE certificates (collagen, gelatin), proof the acerola has no added ascorbic acid, and Kakadu origin and supply (wild-harvest, benefit-sharing).
8. The food classification (jelly confectionery, dessert or other), which sets the permitted additives, any allulose limits, and the NPSC category.

## Open (proposal; not decided)
- Approve the recommended formula for both SKUs. See [decisions.md](decisions.md).
- Bovine (recommended) or marine collagen: still open in decisions.md.
- Whether to pay about A$0.05 more per serve for the PHGG-led "best" fibre and a low-FODMAP certification.
- Ask Finance to re-run COGS at these ingredient costs (A$0.15 to 0.24 per serve, EST), which may push Sand-M to the top of its ฿5 to 9 range.

## Thai 7-Eleven field benchmark (Justin's photos 23 Nov; checked online 24 Nov 2026)
Verify every figure against the packs arriving 26 Nov. Detail and sources: `../daily-bots/reports/2026-11-25-nutritionist.md`.
| Product | Format | Key dose (label / listing) | Fibre or actives | Gel | Price per serve | Note |
|---|---|---|---|---|---|---|
| Doi Kham Fiber Jelly (tamarind-honey) | 25 g sachet | ~11 g fibre ingredients: FOS + inulin 10,000 mg, psyllium 1,000 mg. "13" not confirmed as grams (official page: 5 g carbs, 20 kcal) | Inulin/FOS (high-FODMAP), psyllium, amla | not stated | ฿49 ≈ A$2.09 | Thai dietary supplement; added vit C 100% + B6 60% Thai RDI. [doikham.co.th](https://www.doikham.co.th/product/fiber-jelly-tamarind-honey-flavor) |
| Pananchita Per Peach / Per Melon ("Fiber Buk") | 50 g spout pouch | ~10.8 g fibre (photo); sister Per Buk lists 11,000 mg | FOS, inulin, psyllium, gum arabic, oat beta-glucan, chitosan, B. coagulans, garcinia, ascorbic acid | **Konjac** ("บุก" in name) | ฿49 to 59 ≈ A$2.09 to 2.51 | Closest to our pouch format and peach flavour; stevia |
| Jejuvita Gluta Glassy (lychee-rose) | 25 g strip | ~10 g fish collagen (photo, not confirmed online); sister product lists 10,000 mg collagen tripeptide + 250 mg glutathione | Fish collagen, glutathione | not stated | sister ≈ ฿39 ≈ A$1.66 | Collagen stick benchmark |
| Posh Medica Jelly Fiber (tamarind) | 25 to 28 g sachet | 10,000 mg fibre + probiotics (pack, per review) | Tamarind fibre blend | not stated | ฿39 ≈ A$1.66 | "0% sugar" |
| Nuui Fiberry Jelly | 25 g | 6,000 mg | FOS, psyllium, inulin, GOS | not stated | n/f | Xylitol |
| Body Shape EZE JellyTokz | 25 g | ~3.6 g fibre (photo) | | | | Low dose |
| Sand-M Jelly Me Cuti Activ Fiber | 30 g stick | 7 g, mostly acacia | | Konjac + carrageenan + LBG | ฿20 ≈ A$0.85 | see section 1 |

**Implication (25 Nov):** the Thai 10 to 13 g comes from inulin/FOS, psyllium and konjac, in the Thai *supplement* category with added vitamins. None of that maps to an AU general food. Keep 7 g as the core; see "10 g fibre question" below.

## 10 g fibre question (Nutritionist bot, 25 Nov 2026; proposal, Justin decides)
- **Feasibility:** 10 g label (design ~11 g, ~12.2 g of fibre ingredients) is ~49% w/w in a 25 g stick (not realistic), ~41% in 30 g (high risk), 30 to 35% in a 35 to 40 g stick (trial-able, similar density to today's 7 g/30 g), ~10% in a 120 g pouch (easy). Resistant dextrin-led only; cap acacia at ~2.5 g.
- **GI:** 10 g of RD/acacia/PHGG is tolerable for most adults. 10 g of inulin/FOS often brings gas and bloating.
- **Cost (EST):** ingredients A$0.15 (7 g) → A$0.18 (10 g); landed +A$0.08 to 0.11 a serve with the bigger stick ([finance.md](finance.md) section 10).
- **Claims:** no FSANZ tier above "excellent source" (≥7 g); 10 g adds only a bigger number.
- **Recommendation:** Good: 6 g. **Better (recommended): 7 g core stick now, and ask factories to sample a 10 g RD-led option** (35 to 40 g stick or pouch). Best: a separate 10 g pouch/40 g stick SKU after the ad test.
- **Tombow note (24 Nov):** its stick line can't use pectin, gellan or gelatin and proposes LBG + carrageenan + xanthan. A soft LBG + xanthan (+ a little iota) gel may be squeezable; a firm kappa + LBG gel is not. Open in [decisions.md](decisions.md).
- Tasting protocol for the 26 Nov samples (8 to 10 tasters, blind, 1 to 9 hedonic + JAR + texture + bench tests): see the 25 Nov report.
