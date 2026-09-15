# Evidence, authority and deliberate writes

## Cite inspected sources

Use `architecture` or `application`, root-relative path, section anchor/heading (lines when useful), and Git revision when available. Report each root's working-copy status: clean, dirty, no commit, or unknown. Inspect relevant untracked and modified content too; a commit hash alone does not describe it. In an authorized local run record retain the relevant diff or a local snapshot identifier for dirty evidence; otherwise state that exact working-copy evidence was not retained. Never claim a revision/status you could not determine.

Separate **documented intent**, **observed implementation**, **recommendations** with tradeoffs, **assumptions**, and **unresolved decisions** using ordinary headings or labels, not a new authority taxonomy. Cite code only if inspected; reported behavior without inspection is a report, not verification. Missing evidence gets a focused architect question, not an invented citation.

Existing ADR status, review and exception processes determine authority. Cite the applicable status/process. Unknown authority stays unknown; filenames, commits, interview preferences, generated drafts and successful builds do not establish approval. For conflicting decisions with unclear precedence, cite both, identify the responsible architect's decision, and block dependent choices. For a boundary exception, follow the documented process or ask how approval is obtained; keep the request outstanding until decision evidence exists.

## Recheck and resume

Before updates and relevant follow-ups (including a reopened saved plan), re-resolve roots and re-read cited current sources. Compare revision **and working-copy content/status** with the saved evidence, not just the hash. Report changed, missing, inaccessible or unverifiable references and whether each affected conclusion still holds. A saved plan is context, not architectural authority. Do not silently rely on a stale copy; leave dependent advice unresolved when current evidence cannot be verified.

## Authorize and preserve local writes

Before any file write, state exact destination(s), proposed changes and purpose; obtain approval for that scope. Interview answers are decision inputs, not blanket write permission. Check resolved destinations and ancestors against authorized write roots using the discovery guard. Inspect existing files and working changes immediately before editing. Preserve unrelated edits; if content changed since inspection, re-read and reconcile or ask, never reset/replace blindly.

For a saved plan or feedback filename collision, preserve existing content and ask for a different name or explicit overwrite/merge permission. Do not silently choose an overwrite. Re-read the saved artifact or inspect the resulting diff to verify the intended changes and unchanged scope. No automatic commit, issue creation, messages, publication or approval transition. Plans and feedback normally live under `.arc42-work/` in the application workspace and remain local/unapproved; saving elsewhere needs an agreed local path.

## Report checks honestly

Return changed paths, diff (or patch), assumptions, unresolved decisions, and actual check results: command, working directory, exit status, diagnostics, and produced artifacts. Distinguish passed, failed, blocked and not run. Review text/decision/diagram meaning separately from successful rendering; neither a structural test nor rendering proves architectural approval or agent behavior.
