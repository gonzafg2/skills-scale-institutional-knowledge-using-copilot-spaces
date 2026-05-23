# OctoAcme — RACI Responsibility Mapping Template

## Purpose
Provide a lightweight, reusable matrix to clarify who is **Responsible**, **Accountable**, **Consulted**, and **Informed** for key activities across common project phases. Use this template at project kickoff or whenever handoff clarity is needed.

## When to use
- At project kickoff to align the team on ownership before work begins.
- When scope expands or new roles join mid-project.
- During retrospectives when accountability gaps surfaced as an issue.

## RACI Key

| Letter | Meaning |
|--------|---------|
| **R** | **Responsible** — Does the work |
| **A** | **Accountable** — Owns the outcome; there should be exactly one A per activity |
| **C** | **Consulted** — Provides input before or during the work |
| **I** | **Informed** — Notified of progress or completion |

---

## RACI Matrix Template

Replace role columns with the actual roles on your project. Add or remove rows to match your phase activities.

| Activity | PM | PdM | Dev | QA / Testing | QA Automation | UX/UI | DevOps | Business Owner | SME | End User |
|----------|----|-----|-----|-------------|---------------|-------|--------|----------------|-----|----------|
| **Initiation** | | | | | | | | | | |
| Define problem statement & business case | C | R | I | I | I | I | I | A | C | I |
| Stakeholder identification | R | C | I | I | I | I | I | A | C | I |
| Go/no-go decision | C | C | I | I | I | I | I | A | C | I |
| **Planning** | | | | | | | | | | |
| Backlog creation & prioritization | C | R | C | C | C | C | I | I | C | C |
| Definition of Done agreement | R | C | C | A | C | I | I | I | I | I |
| Definition of Ready agreement | R | C | C | C | C | I | I | I | I | I |
| Risk register setup | A | C | C | C | C | C | C | I | C | I |
| Release plan & milestones | A | C | C | C | C | C | C | I | I | I |
| **Execution** | | | | | | | | | | |
| Feature design & UX prototypes | C | C | C | I | I | A | I | I | C | C |
| Feature implementation | C | I | A | I | I | C | C | I | I | I |
| Automated test authoring | I | I | C | C | A | I | C | I | I | I |
| Manual QA & acceptance testing | I | C | C | A | C | I | I | I | I | C |
| CI/CD pipeline management | I | I | C | I | C | I | A | I | I | I |
| Decision logging | A | C | C | C | C | C | C | I | C | I |
| **Release** | | | | | | | | | | |
| Release readiness sign-off | A | C | C | C | C | I | C | I | I | I |
| Deployment execution | C | I | C | I | I | I | A | I | I | I |
| Rollback execution (if needed) | A | I | C | I | I | I | R | I | I | I |
| Release communications | A | C | I | I | I | I | I | I | I | I |
| **Close & Retrospective** | | | | | | | | | | |
| Retrospective facilitation | A | C | C | C | C | C | C | I | I | I |
| Action item ownership | A | C | C | C | C | C | C | I | I | I |
| Lessons learned documentation | R | C | C | C | C | C | C | I | C | I |

---

## Usage Notes

- **One Accountable per row**: If you have multiple A's in a row, resolve the ambiguity before the work starts.
- **Minimize C's**: Too many Consulted entries slow decisions. Only consult those whose input is genuinely required.
- **Review at milestones**: Ownership can shift across phases—revisit this matrix at each major milestone or when the team changes.
- **Link to the risk register**: Activities with unclear ownership are themselves a project risk. Log them if unresolved.

## Related Documents
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [Definition of Ready](./octoacme-definition-of-ready.md)
- [Dependency Handoff Checklist](./octoacme-dependency-handoff-checklist.md)
- [Decision Log](./octoacme-decision-log.md)
