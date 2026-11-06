# Roadmap Review

**Review date:** 2026-11-06
**Decision owner:** Head of Supply Chain
**Roadmap version reviewed:** v2 (after the audit) → produces v3

## Review Context

> **SCENARIO EVENT (FICTIONAL, S04):** The I04 data quality check for the pilot
> product group shows that **sales history is too incomplete and inconsistent**
> for reliable inventory prediction.

This event was chosen by the group as the material change for the project. It
is not real evidence from the company.

## Outcomes and New Evidence

| ID | New evidence | Source | Type |
|---|---|---|---|
| F08 | Sales history for the pilot product group is too incomplete and inconsistent for prediction | S04 | **Scenario (fictional)** |

No outcome signals had been measured yet. The roadmap was still in its learning
phase.

## Assumptions Confirmed or Rejected

| Assumption or finding | Result | Reason |
|---|---|---|
| F04: integration and data quality are main difficulties | **Confirmed** (in the scenario) | F08 shows data quality blocks prediction for the pilot |
| The first pilot product group has data good enough for prediction | **Rejected** | F08 |
| I01 can move from learning to an approach decision soon | **Rejected for now** | The approach depends on usable data (I04 gate) |

## Initiative Decisions

| Initiative | Continue / adapt / advance / pause / stop | Reason | Approved change | Communication impact |
|---|---|---|---|---|
| I04: Make the data ready | **Adapt** | The current pilot group failed the data gate | Check whether another product group has better data; switch the pilot if so | Data is the main bottleneck; Obj 3 is now the main focus |
| I01: Safety stock in line with demand | **Adapt** | Its stop rule says pause, but part of its learning needs no data | Continue only the learning that needs no data (current parameter process, why the plan does not turn into inventory actions, O05). **The approach decision (AI or non-AI) is paused** until the I04 gate is passed | No recommendations or results expected soon |
| I02: Promotions and seasonal peaks | **Pause** (stays in Next) | Depends on I04, which failed | No work until the I04 gate is passed | No change in what was promised (it was already Exploratory) |
| I03: Finance view | **Advance** (Later → Now), limited to confirming the need | Needs no data; capacity freed up by pausing part of I01 and I02 | Only "ask finance whether the need exists" moves to Now. Building anything stays an option | The CFO is asked directly about the need |

## Updated Risks, Dependencies, and Commitments

- **Risk raised:** data quality is now a confirmed blocker (scenario), not just
  a risk.
- **New dependency:** a new pilot product group must have usable sales history.
- **New risk:** no product group may have good enough data. In that case I04
  becomes a data-fixing effort and the whole roadmap slows down.
- **Commitments changed:**
  - I01 "Committed" now covers only the learning that needs no data (narrowed).
  - I03 "ask finance" is now **Committed** learning (previously an Option).
  - No dates or targets were added.
- **Previous version kept:** v2 placements are recorded in the `roadmap.md`
  change history and in `roadmap-decision-log.md`.

## Next Review Trigger

The next review happens at whichever comes first:

1. Data check results for the alternative product groups (I04).
2. Finance's answer on whether the need exists (I03).
3. The Head of Supply Chain's capacity decision.
