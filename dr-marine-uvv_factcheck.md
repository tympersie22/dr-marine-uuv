# Dr.Marine UVV — Claims Fact-Check

**Prepared:** 11 July 2026 · **Scope:** the six claims in §9 of the concept doc, plus the science mechanics driving the simulation.
**Purpose:** clear any claim to green before this is shown to a funder/grant panel. Verdicts and required edits are below; full sources at the end.

---

## Verdict summary

| # | Claim | Prior | New verdict | Action |
|---|-------|-------|-------------|--------|
| 1 | Coral bleaching ≈ MMM+1 °C; DHW 4 / 8 / 12 tiers | ✅ | ✅ **Confirmed, verbatim** | None. Can strengthen with extra tiers. |
| 2 | Ice-ice drivers; 33–35 °C severe; ~99 % Zanzibar dry-season prevalence | ✅ | 🟡 **Prevalence confirmed; mechanism is nuanced** | Keep "illustrative" label; soften causal wording. |
| 3 | Seaweed farming a major income source for women in Zanzibar | 🟡 | ✅ **Confirmed and strong** | Promote to a headline stat. |
| 4 | Dynamite fishing occurs on the Tanzanian coast | 🟡 | 🔴 **Materially out of date** | Reframe to past tense — do **not** claim it is ongoing. |
| 5 | Specific salinity / DO / turbidity sim ranges | 🟡 | 🟡 **Salinity confirmed; others plausible** | Cite one local field study if published. |
| 6 | Hardware costs / specific models | 🔴 | 🔴 **Still unsourced** | Out of scope until a BOM exists. |

---

## 1 · Coral bleaching threshold & DHW tiers — ✅ Confirmed

NOAA Coral Reef Watch defines heat stress via Degree Heating Weeks (DHW), accumulated over a rolling 12-week window. The published tiers match the doc exactly:

- **4 °C-weeks** — risk of coral bleaching begins.
- **8 °C-weeks** — reef-wide bleaching with mortality of heat-sensitive corals becomes likely.
- **12 °C-weeks** — multi-species mortality becomes likely.
- (Bonus, if you want more range in the gauge: **≥16** severe multi-species mortality in >50 % of corals; **≥20** near-complete mortality in >80 %.)

The simulation's gauge and the doc's wording are accurate. This claim is safe to present as stated. The gauge already carries an "illustrative" label because the real DHW accumulates over 12 weeks while the demo compresses it into ~90 seconds — keep that label.

## 2 · Ice-ice disease — 🟡 Prevalence solid, mechanism needs softer wording

The headline figure holds: a **~99 % ice-ice prevalence** was recorded in a Zanzibar eucheumatoid farm during the dry season (Feb–Mar), with a strong seasonal signal (≈2 % in June, wet season, up to ≈54 % in January). That is well-supported.

**The caution:** the same 2024 field study found **no significant correlation** between ice-ice and most measured parameters — temperature, salinity, pH, and current velocity individually — with only an inverse correlation to ammonium. The "warm water + low salinity" causal story comes largely from *laboratory* work (e.g. Ward et al. 2022), where whitening appears at low salinity (~≤20) and severe damage at 33–35 °C. So the demo's tidy "temperature + low salinity + low circulation → ice-ice risk" is a reasonable teaching simplification, but it overstates how cleanly those variables predict disease in the field.

**Action:** keep the on-screen "illustrative" tag on the ice-ice gauge, and in narration say something like *"warm, low-salinity, low-flow conditions are associated with ice-ice outbreaks"* rather than *"cause"* — defensible and honest.

## 3 · Women & seaweed livelihoods — ✅ Confirmed and strong

This is your strongest impact claim and should be featured, not buried. Current reporting (2025) states that Zanzibar has **~23,000–25,000 seaweed farmers, of whom roughly 80–88 % are women**, and that seaweed is the **third-largest source of income** in Zanzibar. In a context where fewer than half of women are formally employed, it is one of the few reliable independent-income routes available — and it is directly threatened by warming water, which is the exact problem your system addresses. Strong, current, funder-ready.

## 4 · Dynamite / blast fishing — 🔴 Out of date; reframe

This one has changed materially and must not be presented as an ongoing problem. Blast fishing was historically severe on the Tanzanian coast (peaking at an estimated tens of thousands of blasts per year in the 2010s), but enforcement drove a steep decline from ~2016–2018, and in **2025 the government declared blast fishing eradicated** in its Indian Ocean waters — incidents reportedly falling from 20–24 per day in 2023 to effectively zero over the following year.

**Action:** if the pitch mentions it at all, use the past tense as a *success/recovery* framing — e.g. *"reefs recovering from a legacy of blast fishing"* — not *"blast fishing is destroying the reefs."* Claiming it is current would be factually wrong and easy for an informed panel to challenge.

## 5 · Simulated water-quality ranges — 🟡 Salinity anchored, rest plausible

Regional salinity of **~34.1 ‰** is confirmed for Zanzibar waters and matches the sim's default (34.1) and range (33–35). Tropical-lagoon SST in the high-20s °C and the semi-diurnal tidal swings in temperature / DO / pH are consistent with the literature. Specific local numeric ranges for DO and turbidity were **not** pinned to a single Zanzibar field dataset in this pass. The ranges remain plausible placeholders.

**Action:** for anything published, cite one specific Zanzibar/Chwaka Bay water-quality study for the DO and turbidity ranges, or relabel them explicitly as "typical tropical-lagoon values." Do not present them as measured local data.

## 6 · Hardware costs & models — 🔴 Still unsourced

No costing or vendor verification was done in this pass, and none is possible yet because §8 lists no specific priced BOM to check. This stays red until a real parts list with prices exists. Keep §8 labelled "indicative, not a validated BOM" as it already is.

---

## What to change before going public

1. **Dynamite fishing** — rewrite to past-tense recovery framing (highest priority; currently wrong).
2. **Ice-ice** — soften "cause" to "associated with"; keep the "illustrative" gauge label.
3. **Women's livelihoods** — promote to a headline impact stat (~23–25k farmers, ~80 %+ women, 3rd-largest income source).
4. **Water-quality ranges** — either cite a local study or label as "typical tropical-lagoon values."
5. **Bleaching** — no change needed; optionally add the 16/20 tiers for a fuller gauge.
6. **Hardware** — leave as indicative until a priced BOM exists.

None of these block a screen-recording of the *demo* (it's badged SIMULATION). They matter for the spoken narration and any written grant material that goes with it.

---

## Sources

- NOAA Coral Reef Watch — 5km DHW product & thresholds: https://coralreefwatch.noaa.gov/product/5km/index_5km_dhw.php · methodology: https://coralreefwatch.noaa.gov/product/5km/methodology.php
- Ice-ice prevalence, Zanzibar (MDPI *Plants* 2024): https://www.mdpi.com/2223-7747/13/15/2157 · open copy: https://pmc.ncbi.nlm.nih.gov/articles/PMC11314110/
- Women & seaweed livelihoods (UN in Tanzania): https://tanzania.un.org/en/309114-seaweed-farming-pathway-resilient-livelihoods-zanzibar · Africanews (Oct 2025): https://www.africanews.com/2025/10/27/seaweed-farming-in-zanzibar-women-at-the-heart-of-a-blue-revolution/ · Joint SDG Fund: https://www.jointsdgfund.org/article/women-leading-zanzibars-seaweed-transformation
- Blast fishing eradication declared (Xinhua, May 2025): https://english.news.cn/africa/20250523/707c77af58044bab8951c1ca1dd16d80/c.html · The Citizen: https://www.thecitizen.co.tz/tanzania/business/government-declares-win-over-blast-fishing-as-fight-against-illegal-practices-intensifies-5178588 · Hakai Magazine (context): https://hakaimagazine.com/news/in-tanzania-the-fight-against-blast-fishing-is-ramping-up/
- Zanzibar water quality / salinity (PMC): https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4628011/ · Chwaka Bay tidal exchange: https://www.researchgate.net/publication/278668139_Tidal_exchange_in_a_warm_tropical_lagoon_Chwaka_Bay_Zanzibar

*Note: this fact-check covers the domain claims. It does not audit the simulation's code or numeric internals — those are generated client-side and labelled SIMULATION by design.*
