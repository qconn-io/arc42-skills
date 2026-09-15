---
name: arc42-guide
description: Answer architecture questions and plan changes from sources.
---

# Architecture guidance

## When to use
Use for architecture Q&A, feature placement/planning, or follow-up before, during or after implementation. This workflow does not implement application code or write architectural intent. Implementation is a separately requested step in the engineer's normal coding workflow.

## Procedure
1. Read and apply [discovery and scope](../../arc42/references/discovery.md) and [sources and review](../../arc42/references/sources-and-review.md). Finish source inspection with identified roots, relevant intent, provenance and known/unknown authority before advising.
2. **Q&A:** answer the specific question about ownership, rationale, boundaries, constraints or interactions with inspectable citations. If evidence is insufficient, identify the gap and a focused architect question; label any recommendation separately.
3. **Change plan:** use the [plan form](../../arc42/templates/plan.md). Derive placement from documented responsibilities, not from an answer embedded in the invocation. Cover components, relevant APIs/interactions, applicable constraints/decisions and rationale. Present unaffected work even when a dependency is blocked; give alternatives and the decision needed for blocked choices.
4. **Discrepancy or exception:** cite inspected code observations separately from applicable intent. Apply the shared decision/exception rules; keep approval outstanding. Do not redefine architecture to justify code or the requested feature.
5. **Follow-up/resume:** apply the shared recheck procedure to the relevant saved references, including dirty content. Explain what changed and whether prior guidance remains supported; label unverifiable references and dependent uncertainty.
6. Reply conversationally unless saving is requested. For an authorized saved plan, apply the shared write/collision rules to the agreed local path (normally `.arc42-work/plans/<name>.md`), return the verified path and sufficient resume context for any normal coding agent.

## Verification and pitfalls
Check every architectural claim has a citation or uncertainty label; the plan has placement, interactions, rationale and blocking decisions. Confirm application code and architecture are unchanged and only an explicitly authorized plan was saved. A code observation, stale plan or generated recommendation is not accepted intent.
