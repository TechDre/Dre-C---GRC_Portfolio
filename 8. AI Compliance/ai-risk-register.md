# AI Risk Register  
## Use Case: Customer Support Chatbot

This risk register documents **identified risks associated with the use of an AI-powered
customer support chatbot**. The purpose of this document is to practice risk identification,
assessment, and basic mitigation planning from a beginner GRC perspective.

This is a learning artifact and reflects **entry-level risk analysis**.

---

## AI Risk Register – Customer Support Chatbot

| Risk ID | AI Use Case | Risk Description | Impact | Likelihood | Risk Rating | Existing Controls | Residual Risk | Notes |
|-------|------------|------------------|--------|------------|-------------|------------------|---------------|------|
| AI-001 | Customer Support Chatbot | AI may provide incorrect or misleading responses to customers | Medium | Medium | Medium | Human review of chatbot responses, user disclaimers | Low | Chatbot is not used for legal or financial advice |
| AI-002 | Customer Support Chatbot | Personal or sensitive data may be exposed through user interactions | High | Medium | High | Data masking, access controls, and logging | Medium | Assumes data handling policies are enforced |
| AI-003 | Customer Support Chatbot | Users may over-rely on AI responses without human verification | Medium | Medium | Medium | Human Escalation to human support, clear AI labeling | Low | Human oversight is required |
| AI-004 | Customer Support Chatbot | Bias in training data may lead to unfair or inconsistent responses to end users | Medium | Low | Low | A cadence should be established to review chatbot responses and feedback mechanisms | Low | Bias testing should be limited at this stage |

---

## Assumptions & Limitations

- This assessment is based on a **general customer support chatbot use case**
- No sensitive regulated data (e.g., medical or financial) is processed
- Risk ratings are qualitative and intended for learning purposes only
- Controls listed are conceptual and not validated

---

## Purpose of This Document

This risk register demonstrates:
- Risk identification for AI systems
- Basic impact and likelihood assessment
- Understanding of residual risk
- Clear documentation and assumptions
