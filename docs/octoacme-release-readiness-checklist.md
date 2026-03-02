# OctoAcme — Release Readiness Checklist

## Purpose
Provide a structured owner table and checklist to confirm all parties have completed their pre-release responsibilities before every deployment.

## How to Use
Complete this checklist before each release. Each owner should confirm their item(s) before the Release Manager proceeds to production deployment. See the [Release & Deployment Guide](octoacme-release-and-deployment.md) for full deployment steps and rollback procedures.

> See also: [Roles and Personas](octoacme-roles-and-personas.md) · [QA Strategy Template](octoacme-qa-strategy-template.md)

---

## Owner Table

| Area | Owner | Responsibility |
|---|---|---|
| Code & Build | Developers | All PRs merged; CI and security scans passing |
| Acceptance Criteria | QA Lead / Product Manager | All acceptance criteria met and verified |
| Test Execution | QA Lead | Smoke, regression, and integration tests passed in staging |
| Release Notes | Release Manager | Release notes drafted and reviewed |
| Deployment Window | Release Manager | Window scheduled and communicated to stakeholders |
| Rollback Plan | Release Manager + Developers | Rollback / mitigation plan documented |
| Stakeholder Notification | Release Manager / Project Manager | Stakeholders informed of release date, scope, and expected impact |
| Business Approval | Product Manager | Feature sign-off and acceptance confirmed |
| Requirements Traceability | Business Analyst | Requirements mapped to delivered features (see [Requirements Traceability Checklist](octoacme-requirements-traceability.md)) |

---

## Pre-Release Checklist

### Code Readiness
- [ ] All PRs for this release are merged to the target branch
- [ ] CI pipeline passing (tests, linting, security scans)
- [ ] No open critical or blocking defects

### Quality Readiness
- [ ] All acceptance criteria met and documented
- [ ] Smoke tests prepared and passing in staging
- [ ] QA Lead has provided quality sign-off

### Release Preparation
- [ ] Release notes drafted and reviewed
- [ ] Deployment window scheduled and communicated
- [ ] Rollback / mitigation plan documented
- [ ] Staging deployment verified

### Stakeholder Readiness
- [ ] Product Manager has confirmed feature sign-off
- [ ] Stakeholders notified of deployment window and release scope
- [ ] Support team briefed (if applicable)

---

## Post-Release Checklist
- [ ] Production deployment verified
- [ ] Post-deploy smoke tests passed
- [ ] Release announcement sent to stakeholders
- [ ] Monitoring dashboards checked for anomalies
- [ ] Any incidents triaged and documented (see [Risk Management & Communication](octoacme-risks-and-communication.md))
