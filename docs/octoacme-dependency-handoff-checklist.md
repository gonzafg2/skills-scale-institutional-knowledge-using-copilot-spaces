# OctoAcme — Dependency Handoff Checklist

## Purpose
Ensure that work passing between teams, roles, or systems is transferred clearly, completely, and with no gaps in ownership. Use this checklist whenever a deliverable, environment, or piece of work transitions from one owner to another—especially across team boundaries.

## When to use
- Handing off a feature branch from Developer to QA for testing.
- Transferring a deployment artifact from QA to DevOps for release.
- Passing infrastructure configuration from DevOps to a downstream team.
- Sharing design specifications from UX/UI Designer to Developers for implementation.
- Any cross-team dependency surfaced in the risk register or project board.

---

## Pre-Handoff: Sender Checklist

The **sending** team or role completes this before flagging work as ready for the receiver.

### Completeness
- [ ] The work item is fully described and acceptance criteria are written.
- [ ] All linked issues, tickets, or PRs are referenced and accessible to the receiver.
- [ ] Required documentation (runbooks, design specs, test data, config notes) is attached or linked.
- [ ] Outstanding known issues or limitations are documented, not silently passed on.

### Quality Gate
- [ ] Automated tests pass in CI (or failures are documented with a clear rationale for handing off anyway).
- [ ] The deliverable meets the agreed Definition of Done or the subset agreed for this handoff stage.
- [ ] Security scanning or compliance checks relevant to this artifact have been completed.

### Environment & Access
- [ ] Receiver has access to all environments, tools, and credentials needed to continue the work.
- [ ] Environment-specific configuration (secrets, feature flags, environment variables) is documented.
- [ ] Any infrastructure dependencies are provisioned and verified by DevOps/Infrastructure.

### Communication
- [ ] A named receiver (individual or team) has been identified and has confirmed availability.
- [ ] Handoff has been announced in the agreed channel (e.g., project board status update, Slack, PR comment).
- [ ] A due date or SLA for the receiver to begin has been agreed and recorded.

---

## Post-Handoff: Receiver Checklist

The **receiving** team or role completes this upon accepting the work.

### Intake
- [ ] Reviewed the handoff description and all linked artifacts.
- [ ] Confirmed understanding of acceptance criteria and any known limitations.
- [ ] Raised clarification questions within the agreed SLA (do not begin work on ambiguous items).

### Environment Verification
- [ ] Successfully accessed required environments and tools.
- [ ] Ran a basic smoke test or sanity check to confirm the deliverable is in the expected state.
- [ ] Verified that test data, fixtures, or seed data are present and correct.

### Ownership Transfer
- [ ] Ticket/card ownership updated on the project board.
- [ ] Sender notified that the handoff has been accepted and work has started.
- [ ] Escalation path agreed: if a blocker is discovered, who is the contact on the sending side?

---

## Cross-Team Dependency Escalation

If a handoff is blocked or delayed, follow this path:

| Level | Action |
|-------|--------|
| **Level 1** | Receiver contacts sender directly via agreed channel. |
| **Level 2** | Both PMs discuss and adjust timeline or scope; risk register updated. |
| **Level 3** | Business Owner or Sponsor engaged for priority resolution. |

Record all escalations in the [Decision Log](./octoacme-decision-log.md) and the risk register.

---

## Common Handoff Scenarios

### Developer → QA / Testing
- Branch or build artifact reference provided.
- Test environment URL and credentials confirmed.
- Known defects or test edge cases documented in the ticket.
- Feature flag states documented if relevant.

### QA / Testing → DevOps (Release)
- Test summary report and sign-off provided.
- No open P1/P2 defects without documented waiver and PM approval.
- Release notes draft provided or linked.
- Rollback procedure reviewed and confirmed with DevOps.

### UX/UI Designer → Developer
- Final design file version linked (not a draft).
- Component-level annotations and responsive breakpoints documented.
- Edge cases and empty/error states designed and included.
- Open design decisions or outstanding feedback items flagged explicitly.

### DevOps → Downstream / Operations
- Infrastructure-as-code changes reviewed and merged.
- Runbook updated to reflect new configuration.
- Monitoring alerts and dashboards validated for new release.
- On-call handoff completed with incident history summary.

---

## Related Documents
- [RACI Responsibility Mapping](./octoacme-raci-template.md)
- [Definition of Ready](./octoacme-definition-of-ready.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
