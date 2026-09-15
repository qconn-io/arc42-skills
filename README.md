---
name: arc42-skills
description: Standalone distribution of the three arc42 architecture-authoring skills (arc42-author, arc42-guide, arc42-feedback) plus shared references and templates. For Codex CLI only; MIT-licensed. Human review of authored architecture remains required and is not replaced by these skills.
license: MIT
---

# arc42-skills

Standalone, production-ready skill bundle extracted from the `ai-ready-arc42-pilot` pilot. It ships the three portable Codex skills exactly as used in that pilot, plus their shared `.agents/arc42/` references and templates so installation preserves the full context those skills reference.

No tests are included; this repo is the consumable artifact, not the pilot verification environment (`tests/`, `.arc42-work/`, `example-app/`, `docs/`, `walkthroughs/` remain in the pilot repo only).

## What is included

| Skill directory | Skill file | Shared references/templates |
|---|---|---|
| `skills/arc42-author/` | `SKILL.md` | `skills/arc42-support/references/` (arc42-placement, discovery, interview, sources-and-review) |
| `skills/arc42-guide/` | `SKILL.md` | `skills/arc42-support/templates/` (feedback.md, plan.md) |
| `skills/arc42-feedback/` | `SKILL.md` | (same shared folders; installed together) |

The shared `arc42-support/` folder mirrors `.agents/arc42/` from the pilot. When a user installs any of the three skills into their Codex `.claude/skills/` (or `.agents/skills/`) directory, the references and templates travel with them so skill instructions that point to `.agents/arc42/references/...` or `.agents/arc42/templates/...` resolve correctly.

Reference model for packaging: [mattpocock/skills](https://github.com/mattpocock/skills) (MIT, per-skill `SKILL.md` with YAML frontmatter, no hidden dependencies, no custom installer).

## Installation

Copy the three named skill directories (`arc42-author`, `arc42-guide`, `arc42-feedback`) together with the `arc42-support/` directory; do not split references/templates from the skills. Preserve unrelated installed skills; these are additive.

Example (Codex CLI consumer repo):

```sh
# From this repo root into your Codex skills directory
mkdir -p ~/.claude/skills
cp -r skills/arc42-author skills/arc42-guide skills/arc42-feedback skills/arc42-support ~/.claude/skills/
```

No build, no package manager, no global install required. The skills are plain `SKILL.md` files with embedded instructions; they load when the Codex CLI discovers them.

## Scope and limitations

- Supported client: Codex CLI only. Individual scenario evidence (not a blanket promise) determines what passed in the pilot.
- Licensing: MIT (this repo and the three skills). Dependencies referenced by the skills (e.g., `openspec`) keep their upstream licenses; see the pilot's `THIRD_PARTY_NOTICES.md` for attribution.
- The pilot repo (`ai-ready-arc42-pilot`) retains the synthetic Spring Boot application, documentation rendering pipeline, Python verification tests, and walkthrough evidence. That evidence is not reproduced here.
- Actual authored architecture requires experienced-human review; the skills assist but do not grant authority. See `skills/arc42-author/SKILL.md` for the authority-guardrail rules.

## Source and attribution

- Pilot source: `ai-ready-arc42-pilot` (same author, MIT for these skills).
- Shared references/templates: `.agents/arc42/` from that pilot.
- Skill structure and YAML frontmatter follow the convention established by `mattpocock/skills`.
