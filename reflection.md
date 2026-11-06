# Reflection

Answers to the reflection questions in `07-project-handout.md`.

## 1. Which roadmap item had the weakest evidence?

**I03 (a finance view of inventory value and risk).** No source showed that
finance actually has this problem. S01 only names finance as a user group, so
the need stayed an assumption. That is why I03 was placed in Later, and later
moved to Now only to *ask* finance whether the need exists.

## 2. Where did a proposed solution initially hide the real opportunity?

The idea started as "build an **AI module** for demand planning". The evidence
showed that the real problems were **safety stock and reorder points set
manually** (F05) and **poor preparation for promotions and seasonal peaks**
(F06). A simpler non-AI method, such as IBP's built-in safety stock
calculation, might be enough. So whether AI is needed is now an open question
(audit finding 1).

## 3. Which exclusion was hardest to defend?

**Leaving out supplier and production planning.** Stock problems around peaks
may actually come from supplier lead times or production capacity, not only
from inventory settings. Our own roadmap admits this: the I02 stop rule
mentions production capacity, and F06 lists lead time as a possible cause. We
kept the exclusion to stay focused and learn with one pilot first. If I02 shows
the cause is outside inventory, we will revisit this exclusion.

## 4. What changed when confidence, rather than time, defined the horizons?

We did not have to invent delivery dates. When the data check failed (scenario
S04), we could move, pause, and advance items honestly without "missing a
deadline". "Next" means "likely, but open questions remain", not "next
quarter".

## 5. Which new evidence created the most valuable roadmap change?

The (scenario) **data check failure (S04 / F08)**. It confirmed that data
quality is the real bottleneck (F04), paused I02, narrowed I01 to learning that
needs no data, and freed up capacity to ask finance about I03, which gave Obj 2
active work.

## 6. Where did Claude sound more certain than the group had earned?

- Claude rated the evidence for I01, I02, and I04 as **Medium**, although it
  all came from one person, recalled from memory. The audit lowered it to
  Low–Medium.
- Claude presented "an outside source would make your evidence stronger" as if
  it were a course rule. When asked for a reference, it turned out to be
  optional advice.
- Claude's early drafts treated **AI as the intended solution** and named the
  roadmap "AI Inventory Prediction Module", before the evidence showed that AI
  was needed.

All three are recorded in `ai-collaboration-log.md`.
