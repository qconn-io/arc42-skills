---
name: arc42-feedback
description: Capture engineering feedback for architecture review.
---

# Architecture feedback

## When to use
Use for engineering difficulties, missing intent, discrepancies or architecture requests before, during or after implementation. Capture a local unapproved draft; leave architecture documents and approval status unchanged.

## Procedure
1. Read and apply [discovery and scope](../../arc42/references/discovery.md) and [sources and review](../../arc42/references/sources-and-review.md). Establish roots and inspect relevant evidence; distinguish an engineer's reported behavior from verified observations and documented intent.
2. Fill the [feedback form](../../arc42/templates/feedback.md) with task/stage, observation, supporting sources or explicitly missing evidence, engineering impact, proposed change/question and precise decision requested from the responsible architect. Preserve discrepancies and unresolved dependencies rather than resolve authority by inference.
3. Present the draft as `draft` with architectural request `unapproved`. Save only with authorization at an agreed local path, normally `.arc42-work/feedback/<name>.md`. Apply shared write and collision rules: preserve an existing file, ask about another name or explicit overwrite permission. Return the verified saved path, or the inline draft when saving is not authorized.
4. Offer a handoff by passing that draft path and source/root references to `arc42-author`. The architect must recheck evidence and discuss unresolved requests before separately authorizing any documentation draft; feedback is not an accepted decision or approval.

## Verification and pitfalls
Verify the draft exposes evidence, impact and requested decision at any engineering stage, and only the agreed local draft changed. No external issue, message, commit or publication is part of this workflow. A filename or handoff grants no architecture authority.
