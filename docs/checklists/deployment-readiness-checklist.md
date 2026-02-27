# Deployment Readiness Checklist

**Owner:** Deployment Coordinator  
**Related roles:** [Roles & Personas](../octoacme-roles-and-personas.md)  
**Related process:** [Release & Deployment Guide](../octoacme-release-and-deployment.md)

## Purpose
Confirm all prerequisites are met before a release is approved and deployed to production.

---

## Release Information

- **Release name / version:**
- **Release type:** Patch / Minor / Major
- **Target deployment date:**
- **Deployment Coordinator:**
- **Engineering Lead sign-off:**
- **QA sign-off:**
- **Product Manager sign-off:**

---

## Prerequisites

- [ ] All acceptance criteria met and verified by QA
- [ ] All PRs merged to the release branch
- [ ] CI pipeline passing (build, tests, security scans)
- [ ] Release notes drafted and reviewed
- [ ] Database migration scripts tested in staging (if applicable)
- [ ] Feature flags configured correctly for this release

## Approvals

- [ ] Engineering Lead has approved the release
- [ ] QA has signed off on acceptance testing
- [ ] Product Manager has confirmed scope is complete
- [ ] Security review completed (if required)
- [ ] Legal / compliance sign-off obtained (if required)

## Environment & Infrastructure

- [ ] Deployment window scheduled and communicated
- [ ] Staging deployment successful and smoke-tested
- [ ] Configuration and secrets verified for production
- [ ] Backup / snapshot taken (if applicable)
- [ ] Monitoring and alerting confirmed active

## Rollback Plan

- [ ] Rollback procedure documented and accessible
- [ ] Rollback tested in staging (or rollback steps reviewed)
- [ ] On-call engineer notified and available during deployment

## Communication

- [ ] Stakeholders notified of deployment window
- [ ] Support team briefed on upcoming changes
- [ ] Post-deploy announcement prepared

## Post-Deployment Verification

- [ ] Smoke tests passed in production
- [ ] Key metrics and error rates within normal range
- [ ] Stakeholders and support team notified of successful release
- [ ] Release notes published
