# ISO 27001 Risk Register

**Organization:** TechNova Solutions (Fictional)
**Standard:** ISO/IEC 27001:2022 — Clause 6.1.2 (Information Security Risk Assessment)
**Methodology:** Asset-based risk assessment using likelihood × impact scoring (1–5 scale)
**Risk Acceptance Threshold:** Scores below 4 may be accepted; all scores ≥ 4 require treatment
**Document Owner:** GRC / Security Team
**Last Reviewed:** Q1 2026

---

## Risk Register

---

### Risk ID: R-001
**Asset:** Company email system
**Threat:** Phishing emails targeting employees
**Vulnerability:** MFA not enforced for all email accounts
**Likelihood:** 4 – Likely (phishing is pervasive; employees regularly receive targeted emails)
**Impact:** 4 – Major (account compromise could expose sensitive emails and enable lateral movement)
**Risk Score:** 16 (4 × 4)
**Risk Level:** High
**Risk Treatment:** Mitigate
**Treatment Actions:** Enforce MFA on all email accounts; deploy anti-phishing filtering; conduct quarterly phishing simulations
**Relevant SOA Controls:** A.5.17, A.6.3, A.8.5
**Risk Owner:** IT / Security
**Residual Risk:** Medium (after MFA implementation)
**Status:** In Treatment

---

### Risk ID: R-002
**Asset:** Customer database (PII)
**Threat:** External attacker exploits unpatched vulnerability to exfiltrate customer records
**Vulnerability:** Delayed patching cycle; no formal vulnerability management SLA
**Likelihood:** 3 – Possible
**Impact:** 5 – Catastrophic (regulatory fines, reputational damage, customer notification obligations)
**Risk Score:** 15 (3 × 5)
**Risk Level:** High
**Risk Treatment:** Mitigate
**Treatment Actions:** Establish formal patching SLA (Critical: 72 hrs, High: 7 days); implement vulnerability scanning on a weekly cadence; conduct annual penetration test
**Relevant SOA Controls:** A.8.8, A.5.31
**Risk Owner:** Engineering / Security
**Residual Risk:** Medium
**Status:** In Treatment

---

### Risk ID: R-003
**Asset:** Cloud infrastructure (AWS)
**Threat:** Misconfigured S3 bucket or storage resource exposes internal data publicly
**Vulnerability:** No automated cloud security posture management (CSPM) tooling in place
**Likelihood:** 3 – Possible
**Impact:** 4 – Major (public data exposure triggers breach notification and regulatory review)
**Risk Score:** 12 (3 × 4)
**Risk Level:** High
**Risk Treatment:** Mitigate
**Treatment Actions:** Deploy CSPM tooling (e.g., AWS Config, Wiz, or Prisma); enforce infrastructure-as-code (IaC) with security guardrails; conduct quarterly cloud configuration reviews
**Relevant SOA Controls:** A.8.9, A.5.23, A.8.15
**Risk Owner:** Engineering / Cloud Operations
**Residual Risk:** Low
**Status:** Open

---

### Risk ID: R-004
**Asset:** Privileged administrator accounts
**Threat:** Insider threat — privileged user abuses access to modify or exfiltrate data
**Vulnerability:** Privileged access not subject to just-in-time controls or enhanced monitoring
**Likelihood:** 2 – Unlikely
**Impact:** 5 – Catastrophic (full system compromise; high financial and reputational impact)
**Risk Score:** 10 (2 × 5)
**Risk Level:** High
**Risk Treatment:** Mitigate
**Treatment Actions:** Implement privileged access management (PAM); enforce just-in-time (JIT) access for admin roles; enable enhanced logging and alerting on privileged account activity
**Relevant SOA Controls:** A.8.2, A.8.15, A.8.16, A.5.3
**Risk Owner:** IT / Security
**Residual Risk:** Low
**Status:** Open

---

### Risk ID: R-005
**Asset:** Third-party SaaS vendors (e.g., CRM, HR platform)
**Threat:** Vendor suffers a breach that exposes organizational or customer data
**Vulnerability:** No formal vendor security assessment process; no contractual breach notification SLA
**Likelihood:** 2 – Unlikely
**Impact:** 5 – Catastrophic
**Risk Score:** 10 (2 × 5)
**Risk Level:** High
**Risk Treatment:** Mitigate
**Treatment Actions:** Conduct annual vendor security assessments; require SOC 2 Type II reports from critical vendors; include breach notification requirements (≤72 hrs) in contracts
**Relevant SOA Controls:** A.5.19, A.5.20
**Risk Owner:** GRC / Procurement
**Residual Risk:** Medium
**Status:** Open

---

### Risk ID: R-006
**Asset:** Employee laptops and mobile devices
**Threat:** Lost or stolen device leads to unauthorized access to corporate data
**Vulnerability:** No Mobile Device Management (MDM) solution; inconsistent use of full-disk encryption
**Likelihood:** 3 – Possible
**Impact:** 3 – Moderate (access to email and files; potential PII exposure)
**Risk Score:** 9 (3 × 3)
**Risk Level:** Medium
**Risk Treatment:** Mitigate
**Treatment Actions:** Deploy MDM solution; enforce full-disk encryption on all endpoints; enable remote wipe capability; update Acceptable Use Policy
**Relevant SOA Controls:** A.8.1, A.7.9, A.8.24
**Risk Owner:** IT
**Residual Risk:** Low
**Status:** Open

---

### Risk ID: R-007
**Asset:** Production application and infrastructure
**Threat:** Ransomware infection encrypts production systems causing extended outage
**Vulnerability:** Backups not tested regularly; no documented ransomware response playbook
**Likelihood:** 2 – Unlikely
**Impact:** 5 – Catastrophic (extended downtime, revenue loss, customer impact)
**Risk Score:** 10 (2 × 5)
**Risk Level:** High
**Risk Treatment:** Mitigate
**Treatment Actions:** Implement immutable and offline backups; test restoration quarterly; develop ransomware response playbook; deploy endpoint detection and response (EDR)
**Relevant SOA Controls:** A.8.13, A.5.29, A.8.7
**Risk Owner:** IT / Security
**Residual Risk:** Medium
**Status:** Open

---

### Risk ID: R-008
**Asset:** Employee identities and access credentials
**Threat:** Credential stuffing or password spraying attack gains unauthorized access
**Vulnerability:** Weak password policy; no account lockout threshold; MFA not universally enforced
**Likelihood:** 3 – Possible
**Impact:** 4 – Major
**Risk Score:** 12 (3 × 4)
**Risk Level:** High
**Risk Treatment:** Mitigate
**Treatment Actions:** Enforce strong password policy; implement account lockout after failed attempts; deploy MFA across all systems; deploy enterprise password manager
**Relevant SOA Controls:** A.5.17, A.8.5, A.5.15
**Risk Owner:** IT / Security
**Residual Risk:** Low
**Status:** In Treatment

---

## Risk Summary

| Risk Level | Count |
|------------|-------|
| High (≥ 9) | 7 |
| Medium (4–8) | 1 |
| Low (1–3) | 0 |
| **Total** | **8** |

---

## Methodology Notes

- **Likelihood Scale:** 1 = Rare, 2 = Unlikely, 3 = Possible, 4 = Likely, 5 = Almost Certain
- - **Impact Scale:** 1 = Negligible, 2 = Minor, 3 = Moderate, 4 = Major, 5 = Catastrophic
  - - **Risk Score:** Likelihood × Impact
    - - All risks are linked to applicable ISO/IEC 27001:2022 Annex A controls documented in the Statement of Applicability (SOA).
      - - Risk register is reviewed annually or following a material security event.
