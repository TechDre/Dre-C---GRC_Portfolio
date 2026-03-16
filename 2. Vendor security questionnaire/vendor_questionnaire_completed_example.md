# Vendor Security Questionnaire — Completed Example

**Vendor Name:** Acme Cloud Services, Inc. (Fictional)
**Questionnaire Completed By:** Jane Doe, CISO, Acme Cloud Services
**Date Submitted:** February 14, 2026
**Reviewed By:** GRC Analyst, TechNova Solutions
**Review Date:** February 28, 2026

---

## Instructions

This questionnaire is aligned with NIST SP 800-53 security standards. Please answer all questions as accurately and honestly as possible. If a question does not apply to your organization, mark it as N/A with a brief explanation. Where controls are in development, indicate the expected completion date.

---

## Section 1: Organizational Security Program

**Name:** Jane Doe
**Email:** jane.doe@acmecloudservices.example.com
**Phone Number:** (555) 867-5309

**1. Do you have a formal information security program?**
Yes. Acme Cloud Services maintains a documented Information Security Program governed by our Chief Information Security Officer (CISO). The program is reviewed annually and aligns with SOC 2 Type II requirements.

**2. Do you know what security frameworks you follow?**
Yes. Acme follows SOC 2 (Trust Services Criteria), NIST Cybersecurity Framework (CSF), and ISO/IEC 27001 as guiding frameworks for our security program.

**3. Are you SOC 2 or ISO 27001 Certified? (Evidence: certificate or audit report)**
Yes. Acme Cloud Services holds a SOC 2 Type II certification covering the Security, Availability, and Confidentiality Trust Services Criteria. The most recent audit period covered January 1, 2025 – December 31, 2025. A copy of the audit report is available under NDA upon request.

**4. Do you have a dedicated security team or point of contact?**
Yes. Our security team consists of 4 full-time security professionals, including a CISO, two Security Engineers, and a GRC Analyst. Our primary security contact for vendor inquiries is securityteam@acmecloudservices.example.com.

---

## Section 2: Data Handling & Privacy

**5. What types of customer data do you collect, store, or process?**
Acme processes the following categories of data on behalf of customers: names, email addresses, IP addresses, usage/activity logs, and customer-configured content stored on the platform. No financial data (e.g., payment card numbers) is stored in our primary environment.

**6. Is your infrastructure hosted on premises, in the cloud, or both?**
Acme operates entirely on cloud infrastructure. Production systems are hosted in AWS (us-east-1 and us-west-2 regions) with multi-region failover capabilities.

**7. If applicable, are backups stored securely off-site?**
Yes. Backups are encrypted at rest using AES-256 and stored in a geographically separate AWS region (us-west-2). Backups are retained for 90 days. Restoration is tested quarterly.

**8. How do you protect physical devices that store sensitive data?**
As a cloud-first company, no customer data resides on physical devices. Employee endpoints are managed via MDM (Jamf for macOS, Intune for Windows) with full-disk encryption enforced.

**9. How is customer data encrypted?**
Data is encrypted in transit using TLS 1.2 or higher. Data at rest is encrypted using AES-256. Encryption keys are managed via AWS Key Management Service (KMS) with customer-managed key (CMK) options available for enterprise customers.

**10. How long is customer data retained within your company? (Evidence: log retention policy)**
Customer-generated data is retained for the duration of the contract plus 30 days following termination, after which it is permanently deleted. Audit logs are retained for 12 months. Our data retention policy is available upon request.

**11. What is your data deletion process or policy? (Evidence: Policy)**
Upon contract termination, customer data is deleted from active systems within 30 days and from backup media within 90 days. Customers may submit a deletion request at any time via our support portal. A written confirmation of deletion is provided upon completion.

---

## Section 3: Access Control & Authentication

**12. Who has access to our data, and how is access approved?**
Access to customer data is restricted to authorized Acme personnel on a need-to-know basis. All access requests require manager approval and are provisioned through our Identity Governance tool. Access is reviewed quarterly. Support engineers may access customer environments only with explicit customer consent via a ticketed request.

**13. Do you use Multi-Factor Authentication (MFA) for required users? (Evidence: Policy)**
Yes. MFA is enforced for all employees accessing production systems, administrative consoles, and internal tools. We use hardware FIDO2 tokens for privileged accounts and authenticator apps (TOTP) for standard accounts. Our MFA policy is available upon request.

**14. How do you manage user access and remove access for exiting employees? (Evidence: Policy)**
Our offboarding process triggers automated access revocation within 4 hours of an employee's departure date. All corporate accounts (SSO, email, SaaS tools) are disabled via automated workflows through our IdP (Okta). Our offboarding policy is available upon request.

---

## Section 4: Vulnerability Management & Incident Response

**15. Do you perform regular vulnerability scanning and patching? (Provide policy or screenshots)**
Yes. Acme performs automated vulnerability scanning weekly on all infrastructure using Tenable.io. Critical vulnerabilities are patched within 72 hours, High within 7 days, and Medium within 30 days. Annual penetration tests are conducted by a third-party firm. Scan results and patch records are available to auditors under NDA.

**16. How quickly will you notify us if there is a security breach affecting our data? (Evidence: Policy)**
Acme will notify affected customers within 72 hours of confirming a security incident that affects their data, consistent with GDPR Article 33 requirements. Notification will be provided via the primary contact email on file. Our incident notification policy is referenced in our DPA.

**17. Have you experienced a security incident in the last 12 months?**
Yes, one minor incident occurred in August 2025 involving unauthorized access to a single test account due to a misconfigured access policy. No production customer data was affected. The issue was remediated within 4 hours and a root cause analysis was completed. The relevant entry is reflected in our SOC 2 report.

---

## Section 5: Business Continuity

**18. Do you have a business continuity or disaster recovery plan? (Evidence: Report Summary)**
Yes. Acme maintains a Business Continuity Plan (BCP) and Disaster Recovery Plan (DRP). Our target RTO is 4 hours and RPO is 1 hour for production services. DR tests are conducted semi-annually. A summary of the most recent DR test is available upon request.

---

## Section 6: Third-Party & Subprocessor Risk

**19. Do you work with any third-party vendors that will access or process our data?**
Yes. Acme uses the following sub-processors: AWS (infrastructure), SendGrid (transactional email), Datadog (monitoring and logging), and Stripe (billing). A complete and current sub-processor list is available at acmecloudservices.example.com/legal/subprocessors.

**20. Do contractors or third parties receive the same security training?**
Yes. All contractors are required to complete Acme's security awareness training within the first week of engagement and annually thereafter. Contractors are subject to the same acceptable use and security policies as full-time employees.

---

## Section 7: Compliance & Insurance

**21. How do you ensure compliance with data protection laws (GDPR, HIPAA, state privacy laws, etc.)?**
Acme conducts annual compliance gap assessments against GDPR and CCPA requirements. We have a designated Data Protection Officer (DPO) and maintain a Records of Processing Activities (RoPA). We are not a HIPAA Business Associate and do not process PHI.

**22. Do you carry cyber liability insurance? (Evidence: Certificate)**
Yes. Acme carries a $5M cyber liability insurance policy through Chubb. A certificate of insurance is available upon request.

**23. Are you willing to sign a Data Processing Agreement (DPA)?**
Yes. Our standard DPA is available at acmecloudservices.example.com/legal/dpa. We are open to customer-specific DPA addendums upon review by our legal team.

---

## Vendor Risk Assessment Summary

| Category | Rating | Notes |
|----------|--------|-------|
| Security Program Maturity | Low Risk | SOC 2 Type II certified; structured security program in place |
| Data Handling & Encryption | Low Risk | AES-256 at rest; TLS 1.2+ in transit; CMK options available |
| Access Control | Low Risk | MFA enforced; quarterly access reviews; automated offboarding |
| Vulnerability Management | Low Risk | Weekly scans; defined patching SLAs; annual pentest |
| Incident Response | Low Risk | 72-hr notification SLA; documented IR process; one minor incident in past year |
| Business Continuity | Low Risk | RTO 4hrs / RPO 1hr; semi-annual DR testing |
| Third-Party Risk | Medium Risk | Multiple sub-processors; recommend reviewing sub-processor list for data residency requirements |
| Compliance | Low Risk | GDPR/CCPA compliant; DPO designated; no HIPAA obligations |
| Insurance | Low Risk | $5M cyber liability policy in place |
| **Overall Vendor Risk Rating** | **Low Risk** | Recommend approval subject to annual reassessment and DPA execution |

---

## Reviewer Recommendation

**Recommendation:** Approved — Proceed with Engagement
**Conditions:** Execute DPA prior to data sharing; confirm sub-processor list annually; request updated SOC 2 report each audit cycle.
**Next Review Due:** February 2027
**Reviewed By:** GRC Analyst, TechNova Solutions
