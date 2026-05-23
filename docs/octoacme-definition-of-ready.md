# OctoAcme — Definition of Ready

## Purpose
Define the minimum conditions a backlog item must satisfy before it enters sprint planning or is pulled into active development. The Definition of Ready (DoR) prevents wasted effort caused by working on under-specified or blocked items.

## Relationship to Definition of Done
The **Definition of Ready** governs *entry* into work: "Is this item ready to start?"
The **Definition of Done** governs *exit* from work: "Is this item complete?"
Both checklists work together to keep work flowing smoothly and quality high.

---

## Definition of Ready — Checklist

An item is **Ready** when all of the following are true:

### Clarity
- [ ] The item has a clear, concise title that reflects what will be delivered.
- [ ] A description explains the *what* and *why* from the user or business perspective.
- [ ] Acceptance criteria are written, testable, and agreed upon by the Product Manager and QA.
- [ ] The item is scoped to a size the team can complete within a single sprint (or it is split).

### Design & UX
- [ ] If a user-facing change, a UX/UI design or wireframe has been reviewed and is linked.
- [ ] Edge cases, empty states, and error states are covered in designs or acceptance criteria.
- [ ] Accessibility requirements are noted where applicable.

### Technical
- [ ] Any technical approach decisions have been made or noted as open items to resolve in the first day of work.
- [ ] External dependencies (APIs, services, teams) are identified and their availability is confirmed.
- [ ] Known infrastructure or environment requirements are documented and provisioned (or scheduled).

### Testing
- [ ] QA has reviewed acceptance criteria and confirmed they are testable.
- [ ] Any test data or environment requirements are identified.
- [ ] The automation strategy for this item is noted (unit, integration, E2E, or manual-only with justification).

### Ownership & Priority
- [ ] The item has a clearly assigned owner (or ownership will be agreed at sprint planning).
- [ ] Priority is set and agreed by the Product Manager.
- [ ] Any blocking items are resolved or have a documented mitigation.

### Estimate
- [ ] The item has been estimated (story points, t-shirt size, or time-based — whichever the team uses).
- [ ] The estimate reflects current knowledge; significant unknowns are flagged in the item.

---

## When to Apply the DoR

| Context | Guidance |
|---------|----------|
| **Sprint / Iteration Planning** | Only pull items that meet the DoR into the sprint. Items that fail the check go back to the backlog with notes. |
| **Backlog Refinement** | Use the DoR as a refinement exit checklist. An item passes refinement when it becomes Ready. |
| **Mid-sprint additions** | Only add unplanned work mid-sprint if it meets the DoR. Emergency work is exempt but must be documented. |

---

## Who is responsible?

| Role | Responsibility |
|------|---------------|
| **Product Manager** | Ensures items are sufficiently described and prioritized before refinement. |
| **Project Manager** | Facilitates the refinement process; ensures the team has capacity to refine items. |
| **Developers** | Raise technical questions early; flag items that lack technical clarity. |
| **QA / Testing** | Confirm acceptance criteria are testable before an item is declared Ready. |
| **UX/UI Designer** | Delivers and links designs before the item is scheduled for development. |

---

## Definition of Ready — Quick Reference Card

```
✅ Clear title and description
✅ Acceptance criteria written and agreed (PM + QA)
✅ Sized to fit in one sprint
✅ UX designs linked (if user-facing)
✅ Dependencies identified and unblocked
✅ Test approach agreed
✅ Estimated
✅ Owner identified
```

---

## Related Documents
- [Project Planning](./octoacme-project-planning.md) — includes Definition of Done
- [RACI Responsibility Mapping](./octoacme-raci-template.md)
- [Dependency Handoff Checklist](./octoacme-dependency-handoff-checklist.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)
