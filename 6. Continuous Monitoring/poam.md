# Plan of Action & Milestones (POA&M)

**Organization:** TechNova Solutions (Fictional)
**System / Scope:** Corporate Information Systems and Cloud Infrastructure
**Framework Alignment:** NIST SP 800-53 Rev. 5 / FedRAMP Moderate
**Document Owner:** GRC / Security Team
**Reporting Period:** Q1 2026
**Last Updated:** March 2026

---

## Purpose

The Plan of Action & Milestones (POA&M) is a key risk management artifact used to document identified security weaknesses, the corrective actions required to address them, and the milestones for implementation. This document supports continuous monitoring activities and demonstrates progress toward a mature security posture.

POA&Ms are required under FedRAMP, FISMA, and NIST RMF and are typically reviewed monthly and submitted to authorizing officials as part of the ongoing authorization process.

---

## POA&M Tracker

| POA&M ID | Weakness Description | Source | NIST 800-53 Control | Risk Level | Responsible Party | Scheduled Completion | Milestones | Estimated Cost | Status | Notes |
|----------|---------------------|--------|---------------------|------------|-------------------|----------------------|------------|----------------|--------|-------|
| POA-001 | Multi-factor authentication (MFA) not enforced on all employee email accounts | Internal risk assessment | IA-2, IA-5 | High | IT / Security | 2026-04-30 | M1: Inventory all accounts (Mar 15) → M2: Enable MFA in pilot group (Mar 31) → M3: Full rollout (Apr 30) | $2,000 (licensing) | In Progress | 60% complete; admin accounts done |
| POA-002 | No formal vulnerability management policy or patching SLA defined | Continuous monitoring review | SI-2, RA-5 | High | IT Operations | 2026-05-15 | M1: Draft policy (Apr 1) → M2: Management review (Apr 15) → M3: Publish and enforce (May 15) | $0 | In Progress | Draft policy under review |
| POA-003 | Cloud storage buckets lack automated misconfiguration detection | Cloud security review | CM-6, CM-7, AU-6 | High | Engineering / Cloud Ops | 2026-06-30 | M1: Evaluate CSPM tools (Apr 15) → M2: Select and deploy tool (May 31) → M3: Establish alert thresholds (Jun 30) | $5,000/year | Open | Tool evaluation in progress |
| POA-004 | No privileged access management (PAM) solution; admin accounts lack JIT controls | Access review | AC-6, AU-9, IA-2 | High | IT / Security | 2026-07-31 | M1: Define requirements (Apr 30) → M2: Vendor evaluation (May 31) → M3: Pilot deployment (Jun 30) → M4: Full rollout (Jul 31) | $12,000/year | Open | Budget approval pending |
| POA-005 | Vendor security assessment process not formalized; no SOC 2 requirements in contracts | Third-party risk review | SA-9, CA-3 | High | GRC / Procurement | 2026-05-31 | M1: Develop vendor questionnaire template (Apr 15) → M2: Identify and tier vendors (Apr 30) → M3: Begin assessments (May 31) | $0 | In Progress | Questionnaire drafted |
| POA-006 | No Mobile Device Management (MDM) solution; full-disk encryption not verified on all endpoints | Asset inventory | MP-4, SC-28, AC-19 | High | IT | 2026-06-15 | M1: Evaluate MDM solutions (Apr 30) → M2: Deploy MDM (May 31) → M3: Enforce encryption policy (Jun 15) | $8,000/year | Open | — |
| POA-007 | Backup restoration not tested; no ransomware response playbook documented | BCP/DR review | CP-9, CP-10, IR-4 | High | IT / Security | 2026-05-31 | M1: Document restoration procedures (Apr 15) → M2: Test restoration from backup (May 1) → M3: Publish ransomware playbook (May 31) | $0 | Open | — |
| POA-008 | No centralized SIEM; limited visibility into privileged account activity and anomalous behavior | Continuous monitoring gap | AU-2, AU-6, SI-4 | Medium | IT / Security | 2026-08-31 | M1: Requirements gathering (May 15) → M2: Evaluate SIEM solutions (Jun 30) → M3: Deploy and configure (Aug 31) | $18,000/year | Open | Budget request submitted |
| POA-009 | Data retention schedule not documented; no automated deletion workflows | Compliance review | MP-6, SI-12 | Medium | Legal / IT | 2026-06-30 | M1: Inventory data types and systems (Apr 30) → M2: Draft retention schedule (May 31) → M3: Implement and communicate (Jun 30) | $0 | Open | — |
| POA-010 | Security awareness training program lacks structure; completion not tracked | HR / Security review | AT-2, AT-3 | Medium | HR / Security | 2026-05-31 | M1: Select training platform (Apr 15) → M2: Load and assign training curriculum (May 1) → M3: Track completion and report (May 31) | $3,500/year | In Progress | Platform selected |

---

## POA&M Status Summary

| Status | Count |
|--------|-------|
| In Progress | 4 |
| Open (Not Started) | 6 |
| Completed | 0 |
| Deferred | 0 |
| **Total** | **10** |

---

## Risk Level Summary

| Risk Level | Count |
|------------|-------|
| High | 7 |
| Medium | 3 |
| Low | 0 |
| **Total** | **10** |

---

## Review & Escalation Process

- POA&M is reviewed **monthly** by the GRC and IT Security teams.
- Items past their scheduled completion date are **escalated to senior management** within 5 business days.
- Completed items require **evidence of closure** (e.g., policy document, screenshot, audit log) before being marked Closed.
- This POA&M is submitted to the Authorizing Official (AO) as part of the continuous monitoring reporting cadence.

---

## References

- NIST SP 800-53 Rev. 5
- NIST SP 800-137 (Information Security Continuous Monitoring)
- FedRAMP Continuous Monitoring Strategy Guide
- OMB Circular A-130
