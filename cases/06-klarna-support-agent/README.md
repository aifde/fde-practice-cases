# 06. Klarna: production AI support, large efficiency gains, and the return of human service

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High for deployment and scale; mixed evidence on service quality and workforce implications |
| Deployment status | Production since 2024, with continued expansion and a later rebalance toward human support for complex cases |
| Customer | Klarna |
| Delivery partner | OpenAI |
| AI surface | Multilingual customer support connected to account, payment, refund, and return workflows |
| Why it is relevant to AI FDE | The system moved into a high-volume customer workflow, connected to operational actions, measured outcomes, and required later boundary changes based on real service experience |

## Operational problem

Klarna serves consumers across many markets and languages. Customer-service requests range from simple order questions to payment disputes, refunds, returns, and identity-related problems. A useful AI system therefore needs more than a knowledge base. It needs account context, reliable actions, policy controls, and a path to a human when the issue is sensitive or unusual.

Klarna launched its OpenAI-powered assistant globally in 2024. The initial public narrative focused on automation and cost. Later company filings and reporting showed a more complete picture: the AI agent remained a major production channel, while Klarna restored stronger human-service options for cases where quality, empathy, or judgment mattered more.

## Delivery approach

The assistant was embedded in Klarna's existing customer-service experience and made available in multiple languages. It could use customer and order information to answer questions and support workflows involving refunds and returns. The system was designed to resolve common issues quickly and escalate when required.

The later operating model became explicitly dual-track. AI handled a large share of routine volume, while higher-skilled human agents handled complex cases. This correction is central to the case. A forward-deployed team must treat production behavior as evidence and revise the automation boundary when the original design harms service quality.

~~~mermaid
flowchart LR
  A[Customer request] --> B[Identity, account, and order context]
  B --> C[AI support agent]
  C --> D{Can the issue be resolved safely?}
  D -->|Yes| E[Answer or approved account action]
  D -->|No or sensitive| F[Human specialist with conversation context]
  E --> G[Resolution, repeat-contact, and satisfaction signals]
  F --> G
  G --> H[Policy, routing, and automation-boundary updates]
  H --> C
~~~

## Evaluation and operating controls

The public sources describe outcome measures such as conversation volume, resolution time, repeat inquiries, share of chats handled, cost savings, and customer satisfaction. They do not publish the full evaluation design.

A robust interpretation of the deployment requires at least four controls:

- Verify account and transaction context before taking an action.
- Restrict automated actions to policies that can be tested and audited.
- Preserve a clear human escalation route, especially for identity theft, disputes, or emotionally charged cases.
- Monitor repeat contact and service quality, not only deflection and cost.

The need to strengthen human service after the initial rollout is evidence that efficiency metrics alone were not sufficient.

## Publicly reported outcomes

OpenAI and Klarna initially reported:

- 2.3 million conversations in the first month.
- Two-thirds of customer-service chats handled by the assistant.
- A 25% reduction in repeat inquiries.
- Average resolution time below two minutes, compared with 11 minutes for the earlier process.
- Work volume described as equivalent to 700 full-time agents.

Klarna's 2025 securities filing later reported that the assistant handled 69% of service chats in the 12 months ending June 30, 2025 and generated an estimated $39 million in 2024 cost savings. The same filing described a dual-track approach that combined continuing AI use with high-quality human support.

Associated Press reporting in 2025 documented the limitation: Klarna still needed skilled human agents for complex situations such as identity theft. This does not make the AI deployment unreal. It makes the case more useful because it shows how a production system must be re-scoped after real-world feedback.

## Why this is a strong AI FDE case

The deployment connected a frontier model to customer identity, operational data, business policies, and account actions at large scale. It also exposed the difference between a launch metric and a durable service design. The most important FDE lesson is not that AI replaced 700 agents. It is that automation boundaries must be monitored and revised based on customer outcomes.

## What remains unproven

- The original public claims did not disclose issue-level performance, sample sizes, or satisfaction methodology.
- The "700 agents" figure describes estimated work capacity, not a controlled labor-productivity study.
- Cost savings do not measure the value of cases that require empathy, investigation, or trust repair.
- Later hiring and service changes make it unsafe to present the 2024 launch as a final operating model.

## FDE role alignment

- **R1. Embedded discovery and trusted partnership**
- **R2. Scoping and end-to-end delivery ownership**
- **R3. Hands-on implementation and systems integration**
- **R4. AI workflow and human-control design**
- **R5. Evaluation and production quality**
- **R7. Adoption and measurable business impact**
- **R8. Reusable patterns and field feedback**

See the [OpenAI and Amazon FDE role framework](../../role-requirements.md).

## References

1. [OpenAI, Klarna's AI assistant](https://openai.com/index/klarna/)
2. [Klarna Group, 2025 securities filing](https://www.sec.gov/Archives/edgar/data/2003292/000200329225000052/klarnagroupplc424b4.htm)
3. [Klarna Group, 2025 annual report](https://s205.q4cdn.com/644747736/files/doc_financials/2025/q4/Klarna-Group-plc-20-F-2025.pdf)
4. [Associated Press, AI call centers still need humans for complex work](https://apnews.com/article/ca87ae77d7c6797ebb2628bd1b532929)
