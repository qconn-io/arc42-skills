# Focused authoring interview

After source inspection, restate only the requested outcome and affected documented responsibilities, constraints and decisions. Accept ordinary language; translate to documentation placement later. If feedback supplied the request, recheck its evidence and preserve its unapproved status.

Ask the smallest consequential question first. Use dependency order where relevant:

1. Goal, scope and quality/constraint consequences that affect the change.
2. Ownership and responsibility boundaries before interface design.
3. Interactions/APIs, data ownership and lifecycle before runtime details.
4. Failure, concurrency, deployment or operational consequences that depend on those choices.
5. Remaining rationale, decision/exception process, and review needs.

For each unresolved dependency, explain why it matters, offer grounded alternatives and tradeoffs as recommendations, and record the user's answer separately from assumed or pending decisions. Wait for the answer before relying on it. If an owner cannot decide, mark dependent choices blocked and draft only unaffected material when authorized.

Depth follows uncertainty and impact: a small well-defined change needs only its concern addressed, not a compulsory tour of all arc42 chapters. Starting from a template does not turn unknown placeholders into facts. Stop interviewing once relevant uncertainties are answered or explicitly left pending, then propose the exact draft scope for approval.
