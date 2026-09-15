# Place and coordinate the draft

Reuse the selected project's existing organization, anchors and naming rather than restructure it. Map only affected concerns:

| Concern | Typical arc42 location |
| --- | --- |
| Goals, stakeholders, quality priorities | 1 Introduction and goals |
| Binding technical/organizational limits | 2 Constraints |
| System boundary and external actors | 3 Context and scope |
| High-level approach and rationale | 4 Solution strategy |
| Responsibilities, ownership and interfaces | 5 Building block view |
| Interaction sequences and failure paths | 6 Runtime view |
| Infrastructure and mapping to environments | 7 Deployment view |
| Shared concepts/policies | 8 Crosscutting concepts |
| Decisions and alternatives | 9 Architecture decisions / existing ADRs |
| Concrete quality scenarios | 10 Quality requirements |
| Risks and unresolved debt | 11 Risks and technical debt |
| Domain terms | 12 Glossary |

Explain why each affected `.adoc`, ADR and `.puml` belongs in the proposed scope. Follow existing ADR conventions; use draft/proposed status under that process. For a changed accepted decision, retain its historical decision/status and propose a superseding draft as that process requires; never present newly generated substance as already accepted. Leave unrelated chapters and user edits alone.

For each changed boundary or interaction, compare the affected prose, decision rationale and every affected PlantUML diagram: same component names, ownership, direction, sequence and failure assumptions. Check links/includes and stable anchors; update impacted diagrams or explicitly report a blocked dependency rather than claim coherence. Use original/local diagram sources, not remote services/includes.

Inspect the project's rendering route and run authorized local checks on the draft; validate AsciiDoc includes and PlantUML diagnostics as well as exit status and expected HTML/SVG artifacts. A read-only source permits a reviewable unified patch/inline draft, not unauthorized application. If rendering that patch requires an authorized temporary output location, ask for it; report checks not run when unavailable. Use the shared check report for results and keep human semantic review and approval pending.
