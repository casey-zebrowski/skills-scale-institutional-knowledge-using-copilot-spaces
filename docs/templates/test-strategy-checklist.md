# Test Strategy Checklist

**Owner:** [QA/Test Lead](../octoacme-roles-and-personas.md#qatest-lead)  
**Used by:** QA/Test Lead, Developers, Business Analyst, Release Coordinator  
**When to use:** Create or update this checklist at the start of each project/sprint and revisit before every release to confirm test coverage is adequate.

---

## Test Strategy Metadata

- Project / release name:
- QA/Test Lead:
- Sprint / milestone:
- Date last updated:

---

## Scope & Objectives

- [ ] Testing scope is defined (what is in scope / out of scope)
- [ ] Test objectives and quality goals are documented
- [ ] Requirements and acceptance criteria reviewed with [Business Analyst](../octoacme-roles-and-personas.md#business-analyst)
- [ ] Entry and exit criteria defined for each test phase

## Test Types & Coverage

- [ ] **Unit tests** – developer-owned; minimum coverage threshold defined
- [ ] **Integration tests** – key integration points identified and covered
- [ ] **Functional / acceptance tests** – mapped to acceptance criteria from requirements brief
- [ ] **Regression tests** – regression suite updated for new features/fixes
- [ ] **Smoke tests** – core happy-path tests for staging and production verification
- [ ] **Performance / load tests** – required if release includes infrastructure or volume changes
- [ ] **Security tests** – required for any authentication, authorization, or data-handling changes
- [ ] **Accessibility tests** – required for user-facing interface changes
- [ ] **Exploratory testing** – scheduled for new or high-risk areas

## Test Environment

- [ ] Test environment(s) identified and configured
- [ ] Test data requirements documented and data prepared
- [ ] External dependencies / stubs / mocks identified

## Defect Management

- [ ] Defect severity/priority definitions agreed with team
- [ ] Defect tracking tool and workflow confirmed
- [ ] Defect triage cadence scheduled
- [ ] Blocking-defect escalation path defined (to [Project Manager](../octoacme-roles-and-personas.md#project-managers))

## Automation

- [ ] Automation targets identified for this sprint/release
- [ ] Existing automated test suite reviewed for relevance
- [ ] New automated tests added or scheduled for new functionality
- [ ] CI integration confirmed (tests run on each PR)

## Test Execution & Reporting

- [ ] Test execution schedule aligned with sprint/release timeline
- [ ] Test execution results recorded
- [ ] Test summary report prepared and shared with team
- [ ] Quality sign-off provided to [Release Coordinator](../octoacme-roles-and-personas.md#release-coordinator) before go/no-go

---

## Test Sign-Off

| Test Phase | Status | Owner | Date |
|---|---|---|---|
| Unit tests | `[ ] Pass` `[ ] Fail` `[ ] N/A` | | |
| Integration tests | `[ ] Pass` `[ ] Fail` `[ ] N/A` | | |
| Acceptance tests | `[ ] Pass` `[ ] Fail` `[ ] N/A` | | |
| Regression | `[ ] Pass` `[ ] Fail` `[ ] N/A` | | |
| Smoke tests (staging) | `[ ] Pass` `[ ] Fail` `[ ] N/A` | | |
| Performance tests | `[ ] Pass` `[ ] Fail` `[ ] N/A` | | |

**Overall quality sign-off:** `[ ] Approved` `[ ] Blocked — see notes`  
**QA/Test Lead signature:**  
**Date:**  
**Notes / open issues:**
