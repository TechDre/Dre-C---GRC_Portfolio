# Statement of Applicability (SOA)

**Organization:** TechNova Solutions (Fictional)
**Standard:** ISO/IEC 27001:2022
**Scope:** Information Security Management System (ISMS) covering cloud-hosted SaaS platform and associated business operations
**Document Owner:** GRC / Security Team
**Last Reviewed:** Q1 2026

---

## Purpose

This Statement of Applicability (SOA) documents the ISO/IEC 27001:2022 Annex A controls evaluated for applicability to TechNova Solutions. For each control, an applicability determination is provided along with a justification. Controls marked as Not Applicable include an explanation for their exclusion.

---

## Organizational Controls (A.5)

| Control ID | Control Name | Applicable? | Justification |
|------------|--------------|-------------|---------------|
| A.5.1 | Policies for information security | Yes | An information security policy framework is required to establish governance and management direction. |
| A.5.2 | Information security roles and responsibilities | Yes | Defined roles and responsibilities are necessary to ensure accountability across the ISMS. |
| A.5.3 | Segregation of duties | Yes | Segregation of duties reduces risk of fraud and error in access to sensitive systems and data. |
| A.5.5 | Contact with authorities | Yes | Contacts with law enforcement and regulatory authorities are required for incident reporting obligations. |
| A.5.7 | Threat intelligence | Yes | The organization monitors threat intelligence feeds to support risk-informed decision-making. |
| A.5.9 | Inventory of information and other associated assets | Yes | Asset inventory is foundational to understanding the scope of information to protect. |
| A.5.10 | Acceptable use of information and other associated assets | Yes | Acceptable use policies govern employee behaviour regarding organizational assets and data. |
| A.5.12 | Classification of information | Yes | Data classification supports appropriate handling of CUI, PII, and other sensitive data. |
| A.5.13 | Labelling of information | Yes | Labelling supports enforcement of data classification policies across systems and documents. |
| A.5.14 | Information transfer | Yes | Controls over data transfer are required to protect information shared with third parties and via email. |
| A.5.15 | Access control | Yes | Access to systems and data must be restricted to authorized individuals based on least privilege. |
| A.5.17 | Authentication information | Yes | Strong authentication controls including MFA are required for all user and privileged accounts. |
| A.5.19 | Information security in supplier relationships | Yes | Supplier and vendor risk management is critical given reliance on third-party cloud services. |
| A.5.20 | Addressing information security within supplier agreements | Yes | Contractual requirements must reflect security obligations for data protection and breach notification. |
| A.5.23 | Information security for use of cloud services | Yes | The organization relies on cloud infrastructure; cloud security controls are directly applicable. |
| A.5.24 | Information security incident management planning and preparation | Yes | Incident management procedures are required to enable timely and effective response to security events. |
| A.5.25 | Assessment and decision on information security events | Yes | A triage and decision-making process is required to distinguish events from incidents. |
| A.5.26 | Response to information security incidents | Yes | Structured response procedures are required for containment, eradication, and recovery. |
| A.5.27 | Learning from information security incidents | Yes | Post-incident reviews support continuous improvement and control effectiveness assessment. |
| A.5.29 | Information security during disruption | Yes | Business continuity planning must incorporate information security controls. |
| A.5.31 | Legal, statutory, regulatory and contractual requirements | Yes | Compliance with GDPR, CCPA, and contractual obligations must be systematically managed. |
| A.5.36 | Compliance with policies, rules and standards for information security | Yes | Internal audits and compliance reviews verify adherence to ISMS policies. |

---

## People Controls (A.6)

| Control ID | Control Name | Applicable? | Justification |
|------------|--------------|-------------|---------------|
| A.6.1 | Screening | Yes | Pre-employment background checks are required for roles with access to sensitive data. |
| A.6.2 | Terms and conditions of employment | Yes | Employment agreements must include information security responsibilities. |
| A.6.3 | Information security awareness, education and training | Yes | All employees require security awareness training to reduce human risk factors. |
| A.6.4 | Disciplinary process | Yes | A disciplinary process reinforces accountability for policy violations. |
| A.6.5 | Responsibilities after termination or change of employment | Yes | Offboarding procedures must ensure timely access revocation and return of assets. |
| A.6.7 | Remote working | Yes | Remote work is standard across the organization and requires specific security controls. |
| A.6.8 | Information security event reporting | Yes | Employees must have a clear mechanism to report suspected security events. |

---

## Physical Controls (A.7)

| Control ID | Control Name | Applicable? | Justification |
|------------|--------------|-------------|---------------|
| A.7.1 | Physical security perimeters | Yes | Physical access controls are required for office space and server infrastructure. |
| A.7.2 | Physical entry | Yes | Entry controls limit physical access to authorized personnel only. |
| A.7.4 | Physical security monitoring | Yes | Security cameras and access logs support detection of unauthorized physical access. |
| A.7.6 | Working in secure areas | Yes | Procedures for working in secure areas protect sensitive systems and data. |
| A.7.7 | Clear desk and clear screen | Yes | Clear desk and screen lock policies reduce risk of unauthorized visual access to information. |
| A.7.9 | Security of assets off-premises | Yes | Employees use laptops and mobile devices off-site; device security controls are required. |
| A.7.10 | Storage media | Yes | Secure handling and disposal of storage media prevents unauthorized data recovery. |
| A.7.11 | Supporting utilities | Yes | Power and cooling infrastructure supporting systems must be protected against disruption. |
| A.7.14 | Secure disposal or re-use of equipment | Yes | Equipment disposal procedures must prevent data recovery from decommissioned hardware. |

---

## Technological Controls (A.8)

| Control ID | Control Name | Applicable? | Justification |
|------------|--------------|-------------|---------------|
| A.8.1 | User end point devices | Yes | Endpoint security controls are required for all devices accessing organizational systems. |
| A.8.2 | Privileged access rights | Yes | Privileged accounts require elevated scrutiny, MFA, and just-in-time access where possible. |
| A.8.3 | Information access restriction | Yes | Role-based access restrictions enforce least privilege and need-to-know principles. |
| A.8.4 | Access to source code | Yes | Development team access to source code must be controlled to prevent unauthorized modification. |
| A.8.5 | Secure authentication | Yes | Secure authentication mechanisms including MFA are enforced across all critical systems. |
| A.8.6 | Capacity management | Yes | System capacity must be managed to prevent availability impacts on the SaaS platform. |
| A.8.7 | Protection against malware | Yes | Anti-malware controls are required across endpoints and server infrastructure. |
| A.8.8 | Management of technical vulnerabilities | Yes | Vulnerability scanning and patching are required to reduce exposure to known exploits. |
| A.8.9 | Configuration management | Yes | Secure baseline configurations are required for all systems and cloud infrastructure. |
| A.8.10 | Information deletion | Yes | Data deletion procedures are required to meet retention policy and regulatory obligations. |
| A.8.11 | Data masking | Yes | Sensitive data (PII) must be masked in non-production environments. |
| A.8.12 | Data leakage prevention | Yes | DLP controls are required to prevent unauthorized transmission of sensitive data. |
| A.8.13 | Information backup | Yes | Regular, tested backups are required to support recovery from data loss events. |
| A.8.15 | Logging | Yes | Security-relevant events must be logged to support monitoring and incident investigation. |
| A.8.16 | Monitoring activities | Yes | Continuous monitoring of systems and user activity detects anomalous and malicious behaviour. |
| A.8.17 | Clock synchronization | Yes | Synchronized time sources are required to ensure accuracy of audit logs. |
| A.8.20 | Networks security | Yes | Network segmentation and controls protect internal systems from unauthorized access. |
| A.8.21 | Security of network services | Yes | Third-party network services must meet security requirements defined in contracts. |
| A.8.24 | Use of cryptography | Yes | Encryption is required for data at rest and in transit containing sensitive information. |
| A.8.25 | Secure development life cycle | Yes | Security must be integrated into the software development process. |
| A.8.28 | Secure coding | Yes | Secure coding standards reduce the introduction of vulnerabilities in the application. |
| A.8.29 | Security testing in development and acceptance | Yes | Security testing including SAST/DAST must be performed prior to production deployment. |

---

## SOA Summary

| Category | Total Controls Evaluated | Applicable | Not Applicable |
|----------|--------------------------|------------|----------------|
| Organizational (A.5) | 22 | 22 | 0 |
| People (A.6) | 7 | 7 | 0 |
| Physical (A.7) | 9 | 9 | 0 |
| Technological (A.8) | 22 | 22 | 0 |
| **Total** | **60** | **60** | **0** |

---

## Notes

- This SOA covers a representative selection of ISO/IEC 27001:2022 Annex A controls most relevant to a cloud-hosted SaaS environment.
- - A full implementation would address all 93 Annex A controls.
  - - Control applicability is subject to annual review and may change based on business scope, technology changes, or risk assessment outcomes.
