# Initiative Register

**Status:** v2, updated after the audit, approved by the group on 2026-11-06
**Links:** Objectives (Obj 1–3) are defined in `strategy-brief.md`.
Opportunities (O01–O05) and findings (F01–F07) are defined in `evidence-map.md`.

**Confidence note:** All evidence comes from one practitioner, recalled from
memory (S01, S03). Confidence is therefore at most **Low–Medium**.

| ID | Opportunity / problem | Objective | Evidence | Expected outcome | Confidence | Risks / gates | Dependencies | Next learning |
|---|---|---|---|---|---|---|---|---|
| I01 | **Keep safety stock and reorder points in line with real demand** (O01; also covers O05) | Obj 1: reduce both stockouts and excess stock | F03, F05 (S01, S03) | Stock levels follow real demand, giving fewer stockouts and less excess stock in the pilot | Low–Medium | Data quality; **gate: a person approves every parameter change** | I04 | How often safety stock and reorder points are changed today; size of the stockout and excess stock problem in the pilot; **why the IBP plan does not turn into inventory actions (O05)**; whether AI is needed or a simpler method (e.g. IBP's built-in safety stock calculation) is enough |
| I02 | **Get stock ready in time for promotions and seasonal peaks** (O02) | Obj 1 | F06 (S03) | Fewer stockouts during peaks and less leftover stock afterwards | Low–Medium | The cause is unclear; **may overlap with I01** if the cause is stock parameters | I04; promotion data from sales | Whether peak problems come from the forecast, lead times, or stock parameters |
| I03 | **Give finance an early view of future inventory value and risk** (O03) | Obj 2: finance visibility of inventory value and risk | **Assumption only**: S01 names finance as a user group, but the need is not evidenced | Finance sees predicted inventory value and risk early enough to act | Low | The need may not exist | Input from finance | Confirm with finance whether the problem exists and what information they need |
| I04 | **Make the data ready for inventory prediction** (O04) | Obj 3: data reliable enough for predictions | F04 (S01) | Data for the pilot passes an agreed quality gate | Low–Medium | Integration with ERP/IBP; **gate: IT security and data access approval**; **gate: data quality before predictions are used** (criteria still unknown) | IT / ERP team | Choose the pilot plant or product group; data quality assessment for the pilot (which data is affected, how much history exists) |

## Continue, Adapt, or Stop Signals

| ID | Continue if… | Stop or adapt if… |
|---|---|---|
| I01 | The pilot shows fewer stockouts **and** less excess stock, with a person approving the changes | Planners reject most recommendations → adapt the approach or stop |
| I02 | The cause of the peak problems is found and is stock-related | The cause is stock parameters → merge with I01. The cause is outside inventory (e.g. production capacity, which is out of scope) → stop or hand over |
| I03 | Finance confirms the need | Finance does not need it → drop the initiative |
| I04 | The data passes the security and quality gates | The data is too poor → pause I01 and I02 until it is fixed |

## Status After the Roadmap Review (v3, 2026-11-06)

After scenario event S04 / F08 (the pilot data failed the quality check), see
`roadmap-review.md`:

| ID | Status | Change |
|---|---|---|
| I04 | Adapted | Check other product groups for better data; switch the pilot if so. Confidence raised to Medium (F04 confirmed by F08) |
| I01 | Adapted | Only learning that needs no data continues (process, O05); the approach decision is paused |
| I02 | Paused | Until the I04 gate is passed |
| I03 | Advanced (Later → Now) | Only "ask finance whether the need exists" |

## Decisions on Opportunities

- **O05** (the plan does not turn into inventory actions) is **merged into I01**
  as a learning question rather than kept as a separate initiative. Its cause is
  unclear and overlaps with O01. (Group decision, 2026-11-06)

## Candidate Approaches

<!-- Keep possible experiments or solutions separate from the initiative itself. -->

These are possible ways to address the initiatives. **None are decided.**

| Initiative | Candidate approach |
|---|---|
| I01 | (a) Use or tune IBP's built-in safety stock calculation (non-AI); (b) AI/ML recommendations for safety stock and reorder points, approved by a person |
| I02 | A model that predicts how much promotions and seasonal peaks increase demand |
| I03 | A finance view of predicted inventory value and risk |
| I04 | Automatic data quality checks on ERP/IBP data for the pilot |
