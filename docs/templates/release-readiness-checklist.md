# Release Readiness Checklist

**Owner:** [Release Coordinator](../octoacme-roles-and-personas.md#release-coordinator)  
**Used by:** Release Coordinator, QA/Test Lead, Tech Lead, Project Manager  
**When to use:** Complete this checklist before every release (patch, minor, or major) to confirm all criteria are met prior to the go/no-go decision.

---

## Release Metadata

- Release name / version:
- Target release date:
- Release type: `[ ] Patch` `[ ] Minor` `[ ] Major`
- Release Coordinator:
- Tech Lead sign-off:
- QA/Test Lead sign-off:

---

## Code & Build

- [ ] All features/fixes included in this release have been merged to the release branch
- [ ] CI pipeline passes (build, unit tests, integration tests)
- [ ] Security scans pass with no critical/high findings
- [ ] Dependency and license checks pass
- [ ] No known blocking defects outstanding (see Defect Log)

## Documentation & Release Notes

- [ ] Release notes drafted and reviewed (see [Release & Deployment Guide](../octoacme-release-and-deployment.md))
- [ ] API / user-facing documentation updated (if applicable)
- [ ] Migration or upgrade steps documented (if applicable)

## Testing & Quality

- [ ] QA/Test Lead has completed test execution (see [Test Strategy Checklist](test-strategy-checklist.md))
- [ ] Smoke-test suite passes on staging environment
- [ ] Regression suite passes
- [ ] Performance / load tests completed (if applicable)
- [ ] Accessibility checks completed (if applicable)

## Stakeholder & Communication

- [ ] Stakeholder Sponsor notified of release date and scope
- [ ] Support / operations team briefed
- [ ] Deployment window communicated to all affected teams
- [ ] Customer-facing announcement drafted (if applicable)

## Rollback & Risk

- [ ] Rollback / mitigation plan documented and tested
- [ ] On-call / incident-response roster confirmed for deployment window
- [ ] Known risks and mitigations listed in the Risk Register

---

## Go / No-Go Decision

| Role | Name | Decision | Date |
|---|---|---|---|
| Release Coordinator | | `[ ] Go` `[ ] No-Go` | |
| Tech Lead | | `[ ] Go` `[ ] No-Go` | |
| QA/Test Lead | | `[ ] Go` `[ ] No-Go` | |
| Project Manager | | `[ ] Go` `[ ] No-Go` | |

**Final decision:** `[ ] Go` `[ ] No-Go`  
**Notes / conditions:**

---

## Post-Release Verification

- [ ] Production deployment succeeded
- [ ] Post-deploy smoke tests pass
- [ ] Monitoring / alerts healthy
- [ ] Release announcement sent to stakeholders
- [ ] Release ticket closed
