# Strategy Brief

**Status:** Draft v1, approved by the group on 2026-11-06
**Decision owner:** Head of Supply Chain
**Roadmap audience:** Head of Supply Chain and CFO (leadership)

## Product Context

This is an inventory prediction capability that adds to an existing ERP and
integrated business planning (IBP) system such as Infor IBP. AI is a candidate
approach; whether it is needed is decided after the learning steps (see
`roadmap.md`). The setting is a
European snack food manufacturer, anonymised and based on practitioner
experience (S01).

The planning system improved strategic and tactical planning. It did not
improve inventory management enough (S01). This module targets that gap
between the plan and the actual inventory.

## Vision

Inventory managers and finance can see future stock risks early and act on
them before stockouts or overstock happen.

## Target Groups and Priority Needs

| Group | Priority need | Source |
|---|---|---|
| Inventory management | Early warning of future stockouts *and* excess stock, with recommendations they can act on | S01 |
| Finance | Visibility of inventory value, working capital tied up, and stock risk | S01 |

## Strategic Choices

| Choice | Decision | Evidence or rationale |
|---|---|---|
| Where we focus | Predicting inventory: future stock levels and the risk of a stockout or overstock | S01: the planning system covered strategic/tactical planning, but inventory management stayed weak |
| How we intend to create value | Early warnings and stock recommendations that a human reviews and approves | Assumption: planners and finance need to trust the output before acting on it |
| Capabilities or advantages | Builds on the existing ERP/IBP data and planning process | S01: the planning system is already in place |
| What we will not pursue | 1. We will **not** develop an IBP system from scratch. 2. **No automatic orders:** the AI only suggests, and a person approves every order. 3. **No changes** to supplier or production planning for now. 4. **No full rollout:** we start with one plant or one product group only. | Group decisions (2026-11-06): keep and extend the existing planning capability, keep human control, and limit scope so learning comes before scaling |

## Objectives and Signals

| Objective | Outcome signal | Baseline | Target or direction | Evidence source |
|---|---|---|---|---|
| Obj 1: Reduce both stockouts and excess stock | Stockout frequency; share of slow-moving or excess stock | Unknown | Both decrease | S01 (problem); S02 (vendor claims only, unverified) |
| Obj 2: Give finance visibility of inventory value and risk | Finance can see the value of predicted inventory and risk per period | Unknown | Available and used in finance reviews | S01 |
| Obj 3: Make data quality reliable enough for AI predictions | Data quality issues found in the inputs to predictions | Unknown | Decreasing; quality gate met before predictions are used | S01 (data quality and integration were the main difficulties) |

*No baselines or targets have been supplied. They stay unknown until real data
is available. Vendor figures from S02 are not used as targets.*

## Evidence Sources (summary)

| ID | Source | Limitation |
|---|---|---|
| S01 | Practitioner experience: an ERP/IBP demand and supply planning implementation (Infor IBP) at a European snack food manufacturer | One person's view of one project, recalled from memory, with no quantitative data |
| S02 | o9 Solutions, Demand Planning web page (accessed 2026-11-06) | Vendor marketing; unnamed customers; no baselines, time frames, or independent verification |
| S03 | Practitioner observation on why inventory did not improve after IBP: (a) safety stock and reorder points were still set manually or rarely updated; (c) promotions and seasonal peaks still caused problems even when the forecast was acceptable | Same person as S01, so not an independent source; recalled from memory, with no quantitative data |

## Constraints, Risks, and Unknowns

**Constraints**
- The existing ERP/IBP system must be reused, not rebuilt.
- A person approves every AI recommendation (group decision).
- Scope is limited to one plant or one product group at first.
- Supplier and production planning are out of scope for now.

**Risks**
- Integration between the AI module and the ERP/IBP system (S01).
- Data quality is not good enough for reliable predictions (S01).
- Inventory managers or finance may not trust the AI output.

**Unknowns**
- How much the two reasons in S03 (manual safety stock; promotions and seasonality) each contribute, and whether there are other causes.
- Current stockout and excess stock levels (no baselines).
- How much sales and inventory history is available, and how good it is.
- Team capacity, budget, and any fixed deadlines.
- Which plant or product group is the pilot.
- The data quality gate's criteria and who approves them.
- Whether AI is needed, or a simpler method is enough.
- Whether privacy, security, or compliance gates apply.
