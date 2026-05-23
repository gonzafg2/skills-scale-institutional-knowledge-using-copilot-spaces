# OctoAcme — Decision Log Template & Guidance

## Purpose
Track significant project decisions so the team can understand *why* choices were made, revisit them if context changes, and avoid re-litigating settled debates. The decision log is a living artifact—start it at kickoff and update it throughout the project.

## When to use a Decision Log entry

Create an entry when:
- A significant technical or product direction is chosen over alternatives.
- A trade-off is made that affects scope, timeline, cost, or quality.
- A key assumption is confirmed or invalidated.
- An escalation reaches a resolution.
- You want to record stakeholder or sponsor alignment on a choice.

Do **not** log:
- Routine day-to-day implementation choices that can be reversed without team discussion.
- Information already captured in a ticket's acceptance criteria or PR description.

## Decision Log Template

Copy the block below into your project decision log file (e.g., `DECISIONS.md` in the project repo or as a section in the project one-pager).

---

```markdown
## Decision — [Short title, e.g., "Use PostgreSQL as primary database"]

| Field | Value |
|-------|-------|
| **ID** | DEC-001 |
| **Date** | YYYY-MM-DD |
| **Status** | Proposed / Accepted / Superseded |
| **Deciders** | @name, @name |
| **Consulted** | @name, @name |
| **Informed** | @name, @name |

### Context
_What situation or problem prompted this decision? What constraints or pressures were relevant?_

### Options Considered

| Option | Pros | Cons |
|--------|------|------|
| Option A | … | … |
| Option B | … | … |

### Decision
_State the chosen option and the primary reason(s) for choosing it._

### Consequences
_What does this decision enable? What trade-offs are accepted? What follow-up actions are required?_

### Superseded By
_If this decision is later reversed, record the ID of the decision that replaces it._
```

---

## Decision Status Lifecycle

| Status | Meaning |
|--------|---------|
| **Proposed** | Under discussion; not yet agreed |
| **Accepted** | Agreed by the deciders; guiding the project |
| **Superseded** | A later decision replaces this one |

## Ownership & Cadence

- **Owner**: Project Manager ensures the log exists and is kept up to date.
- **Contributors**: Any team member can propose an entry; the PM merges it after confirming deciders.
- **Review**: Skim the decision log at sprint reviews and before major releases to confirm decisions are still valid.
- **Location**: Store in the project repository alongside the charter or in this `docs/` folder for cross-project reference.

## Example Decision Entry

```markdown
## Decision — Store user preferences in browser localStorage

| Field | Value |
|-------|-------|
| **ID** | DEC-003 |
| **Date** | 2024-11-12 |
| **Status** | Accepted |
| **Deciders** | @alice (PdM), @bob (Tech Lead) |
| **Consulted** | @carol (UX Designer), @dave (Security) |
| **Informed** | @PM-team |

### Context
We need to persist user UI preferences (theme, column order) across sessions. Backend storage would require a schema change and additional API endpoints.

### Options Considered

| Option | Pros | Cons |
|--------|------|------|
| localStorage | Zero backend changes; fast | Not synced across devices |
| Backend user preferences table | Cross-device sync | 2-week scope increase |

### Decision
Use localStorage for this release. The majority of users work from a single device, and we can revisit cross-device sync in a future sprint.

### Consequences
- Preferences will reset if the user clears browser storage.
- A follow-up story (DEC-003-FOLLOW-UP) is created for cross-device sync in the next quarter.
```

## Related Documents
- [RACI Responsibility Mapping](./octoacme-raci-template.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Project Planning](./octoacme-project-planning.md)
