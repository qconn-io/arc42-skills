---
name: arc42-author
description: Draft architecture changes through a focused interview.
---

# Architecture authoring

## When to use
Use to create or evolve arc42 documentation, start from an incomplete template, or discuss an engineer's feedback with the architect. Produces a reviewable documentation draft, not application implementation or automatic approval.

## Procedure
1. Read and apply [discovery and scope](references/discovery.md) and [sources and review](references/sources-and-review.md). Inspect current relevant text, decisions and diagrams first; identify evidence and summarize affected responsibilities, constraints and existing decisions. Missing/inaccessible material and template placeholders remain unknown.
2. Use the [focused interview](references/interview.md) to clarify ordinary-language intent in dependency order. Distinguish recommendations/tradeoffs from user decisions. Discuss supplied feedback as an unapproved request, rechecking its sources. Apply the shared authority rules to conflicts and boundary exceptions before relying on dependent choices.
3. Use [arc42 placement and coordination](references/arc42-placement.md) to propose the exact affected AsciiDoc, ADR and PlantUML files, reasons, assumptions and unresolved issues. Obtain explicit write-scope approval under the shared write rules before modifying anything; interview answers alone do not authorize writes.
4. Re-read affected sources and existing edits, then produce focused, coordinated draft changes only in that scope. If the selected checkout cannot be written, explain the restriction and offer a reviewable patch or draft in an authorized location (or inline); keep the source unchanged and do not expand permissions.
5. Check all affected text/decisions/diagrams for consistency using the placement reference. Run authorized rendering/checks and present the diff, changed paths and shared actual-check report. Account for every affected artifact, unresolved dependency and check not run; preserve existing approval status pending the responsible architect's review.

## Verification and pitfalls
A small change must not force unrelated chapter completion. Verify the diff preserves unrelated edits and every changed boundary/sequence agrees across affected artifacts. Rendering success and a feedback handoff grant no authority; human meaning review remains separate.
