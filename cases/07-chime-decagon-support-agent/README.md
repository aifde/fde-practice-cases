# 07. Chime and Decagon: regulated customer support across chat and voice

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High that the named system is deployed; performance figures are vendor and customer disclosures without public methodology |
| Deployment status | Production across chat and voice |
| Customer | Chime |
| Delivery partner | Decagon |
| AI surface | Member support, cross-channel memory, policy-driven actions, routing, and continuous customer-experience feedback |
| Why it is relevant to AI FDE | Decagon teams worked alongside Chime product and operations teams, connected the agent to regulated workflows, and iterated behavior while technical teams retained control of core logic |

## Operational problem

Chime needed to scale member support while preserving accuracy, reliability, security, and a member-first experience. The work spans chat and phone, and the underlying issues can involve sensitive account context and actions such as card replacement or deposit-status checks.

Running separate automation systems for chat and voice would create duplicated knowledge, inconsistent policies, and fragmented feedback. Chime wanted one operating model that could resolve structured requests while keeping human and technical teams in control of the harder cases and core business logic.

## Delivery approach

Chime evaluated multiple partners using response accuracy, automation rate, operational efficiency, and support Net Promoter Score. It selected Decagon for both chat and voice.

The deployed design uses a shared knowledge and behavior layer across channels. Conversations contribute to a common feedback loop, so lessons from chat can improve voice and vice versa. Customer-experience teams can adjust agent behavior through natural-language Agent Operating Procedures, while Chime's technical teams retain control over core logic and member experience.

Decagon says its teams worked directly with Chime's product and operations teams. That collaboration enabled rapid feedback, behavior changes, and the use of conversation insights to inform both support and product improvements.

~~~mermaid
flowchart LR
  A[Member request by chat or voice] --> B[Identity and account context]
  B --> C[Shared Decagon agent layer]
  C --> D[Policy and action controls]
  D --> E{Resolve or escalate?}
  E -->|Resolve| F[Approved answer or account action]
  E -->|Escalate| G[Human support with retained context]
  F --> H[Resolution and satisfaction signals]
  G --> H
  H --> I[CX behavior updates and engineering guardrails]
  I --> C
~~~

## System and control design

| Concern | Delivery response described publicly |
| --- | --- |
| Channel consistency | Chat and voice share knowledge, conversation context, and improvement signals. |
| Business rules | Agent Operating Procedures let operations teams describe behavior, while technical teams control core logic. |
| Human handoff | Cases outside the automated path can move to human support with context preserved. |
| Quality | Chime evaluated accuracy, resolution, efficiency, and member satisfaction rather than using deflection alone. |
| Continuous improvement | Product and operations teams worked with Decagon to adjust use cases and agent behavior. |

## Publicly reported outcomes

Decagon's Chime case study reports:

- More than 70% resolution for chat.
- Nearly 70% resolution for voice.
- Hundreds of thousands of messages automated during the first two weeks.
- More than one million calls per month with no reported reliability issues.
- Improvement in member satisfaction compared with other evaluated vendors.

Other Decagon materials report a 60% reduction in support costs and a doubling of member satisfaction. Those figures are not accompanied by the underlying measurement period or methodology, so they should be treated as vendor-reported outcomes rather than independently verified results.

## Why this is a strong AI FDE case

The case involves a regulated business, multiple channels, account-level context, operational actions, technical guardrails, and continuous feedback. It also shows the division of responsibility required in forward deployment: customer-experience teams shape behavior, engineers own hard controls and integrations, and the delivery partner helps both groups turn policy into a production system.

## What remains unproven

- Chime has not published an independent technical report for this deployment.
- Resolution-rate definitions, evaluation samples, and escalation distributions are not public.
- "No reliability issues" is a customer-story statement, not a published availability measure.
- Cost and satisfaction claims require more detail before they can be compared with other support systems.

## FDE role alignment

- **R1. Embedded discovery and trusted partnership**
- **R2. Scoping and end-to-end delivery ownership**
- **R3. Hands-on implementation and systems integration**
- **R4. AI workflow and human-control design**
- **R5. Evaluation and production quality**
- **R6. Security, governance, reliability, and cost**
- **R7. Adoption and measurable business impact**
- **R8. Reusable patterns and field feedback**

See the [OpenAI and Amazon FDE role framework](../../role-requirements.md).

## References

1. [Decagon, Chime customer success story](https://decagon.ai/case-studies/chime)
2. [Decagon, enterprise conversational AI buyer's guide](https://decagon.ai/blog/conversational-ai-platform-for-enterprise)
3. [Chime, SEC registration statement and member-support context](https://www.sec.gov/Archives/edgar/data/1795586/000162828025025059/chimefinancialinc-sx1wq1da.htm)
