# Evidence and Opportunity Map

**Status:** v1, approved by the group on 2026-11-06

## Research Question and Scope

Why did inventory management not improve enough after the IBP implementation,
and where could AI prediction help inventory managers and finance?

**Scope:** A European snack food manufacturer (anonymised) using an ERP/IBP
system (Infor IBP). The focus is inventory management. Supplier and production
planning are out of scope (see `strategy-brief.md`).

## Sources

| Source ID | Source type | Participants / sample | Date | Limitations |
|---|---|---|---|---|
| S01 | Practitioner experience from an ERP/IBP demand and supply planning implementation | 1 person (group member), 1 project | Recalled 2026-11-06 | One person's view, recalled from memory; no quantitative data; anonymised, no confidential data |
| S02 | Vendor web page: o9 Solutions, Demand Planning | Unnamed customer cases and testimonials | Accessed 2026-11-06 | Vendor marketing; customers unnamed or unclear; no baselines, time frames, or independent verification |
| S04 | **SCENARIO (FICTIONAL)**: roadmap review event, the result of the I04 data quality check | Pilot product group data | 2026-11-06 | **Fictional event** introduced for the project's change exercise; not real company evidence |
| S03 | Practitioner observation on why inventory did not improve after IBP | Same person as S01 | Recalled 2026-11-06 | Not independent of S01; recalled from memory; no quantitative data |

## Findings and Insights

| ID | Finding | Source IDs | Interpretation / insight | Contradictions or gaps |
|---|---|---|---|---|
| F01 | Before IBP, demand was planned manually in Excel | S01 | Planning used to depend on manual work | Unknown whether Excel is still used for inventory after IBP |
| F02 | IBP improved strategic and tactical planning | S01 | Mid- to long-term planning is not the main gap | No measurement of how much it improved |
| F03 | IBP did not improve inventory management enough | S01 | The gap lies between the plan and inventory decisions | "Enough" is not quantified; no stockout or excess stock figures |
| F04 | Integration and data quality were the main difficulties | S01 | Any AI prediction depends on fixing or managing the data first | Unknown which data (sales, stock, master data) was affected |
| F05 | Safety stock and reorder points were still set manually or rarely updated | S03 | Inventory parameters do not follow changes in demand, which can cause both stockouts and excess stock | Only one person's view; frequency and impact unknown |
| F06 | Promotions and seasonal peaks still caused stock problems, even when the forecast was acceptable | S03 | The forecast alone is not enough; translating it into stock levels around events fails | Unknown whether the cause is forecast, lead time, or parameters |
| F07 | A vendor claims AI forecasting reduces stockouts and inventory losses (e.g. "60% reduction in stock-outs") | S02 | Suggests the problem is common and that AI approaches exist | Unverified marketing claims; **not used as targets or proof** |

| F08 | **(Scenario)** Sales history for the pilot product group is too incomplete and inconsistent for prediction | S04 | Confirms F04 in the scenario: data quality is a blocker, not only a risk | Fictional; other product groups not yet checked |

## Opportunities

| ID | Affected group and problem | Intended outcome | Supporting findings | Confidence | Unknowns |
|---|---|---|---|---|---|
| O01 | Inventory managers cannot keep safety stock and reorder points up to date as demand changes, leading to both stockouts and excess stock | Stock levels follow real demand | F03, F05 | Medium | How often parameters are updated today; size of the stockout and excess stock problem |
| O02 | Inventory managers cannot prepare stock in time for promotions and seasonal peaks | Fewer stockouts during peaks and less leftover stock afterwards | F06 | Medium | Whether the cause is the forecast, lead times, or stock parameters |
| O03 | Finance cannot see future inventory value and risk early | Fewer working capital surprises | S01 names finance as a user group; **the need itself is an assumption** | Low | Whether finance actually experiences this problem; what information finance needs |
| O04 | ERP/IBP data is not reliable or connected enough to support predictions | Data good enough to trust prediction outputs | F04 | Medium | Which data sources are affected; how much history is available |
| O05 | The IBP plan does not turn into inventory actions | Plan and stock decisions are aligned | F02, F03 | Low | The cause of the gap is unclear (process, tools, ownership, or parameters) |

## Open Gaps

- No direct input from inventory managers or finance; all findings come from one practitioner.
- No quantitative data (stockout rate, excess stock, inventory value).
- Unknown whether Excel is still used for inventory decisions after IBP.
- User trust in AI is not supported by the evidence and stays an open question.
