# 04. BBVA: from a controlled enterprise pilot to bank-wide AI transformation

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High |
| Deployment status | Production, expanded from 3,000 initial licenses in 2024 to organization-wide access and joint solution development |
| Customer | BBVA |
| Delivery partner | OpenAI, alongside BBVA's internal AI, legal, security, compliance, and business teams |
| AI surface | Employee assistants, legal and risk analysis, customer-feedback analysis, software development, and planned customer-facing agents |
| Why it is relevant to AI FDE | The work combined secure rollout, domain-led prototyping, adoption programs, shared components, and a direct field-to-product relationship between BBVA and OpenAI |

## Operational problem

BBVA wanted to move beyond isolated generative-AI experiments without creating uncontrolled use of sensitive banking information. The bank had to support many countries and business functions, meet legal and security requirements, and identify workflows where AI produced more than drafting convenience.

The central delivery problem was therefore organizational and technical at the same time: give domain experts safe access, help them turn ideas into working assistants, review the most valuable use cases, and create a path from employee prototypes to reusable bank-wide systems.

## Delivery approach

BBVA began distributing ChatGPT Enterprise licenses in May 2024. The initial agreement covered about 3,000 employees and included compulsory training, a multi-country community, and feedback channels. Legal, compliance, security, and technology teams were involved from the beginning.

Employees built task-specific GPTs. Examples published by BBVA include a legal assistant for branch questions, a credit-analysis assistant that extracts information from company reports, and a customer-experience assistant that analyzes open-ended survey responses. A central adoption team and a network of champions helped teams test and share useful patterns.

The relationship later expanded from tool adoption into joint transformation. BBVA and OpenAI announced shared work across customer experience, risk, operations, software development, and employee assistance. BBVA also described a move toward standard platforms and components for building and governing intelligent agents.

~~~mermaid
flowchart LR
  A[Business teams and domain experts] --> B[Secure enterprise AI workspace]
  B --> C[Task-specific assistants and prototypes]
  C --> D[Legal, security, compliance, and quality review]
  D --> E[Approved workflow deployment]
  E --> F[Usage and business feedback]
  F --> G[Shared components, training, and agent platform]
  G --> B
~~~

## Governance and adoption design

| Delivery concern | Publicly described response |
| --- | --- |
| Data protection | Enterprise access, confidentiality guidance, and involvement from legal, security, and compliance teams. |
| User capability | Compulsory onboarding, workshops, champions, advanced users, and internal communities. |
| Use-case discovery | Domain experts build against real legal, risk, operations, and customer workflows. |
| Reuse | An internal GPT store and shared agent components make successful patterns discoverable. |
| Scale | The program expanded in stages rather than opening every workflow at once. |

## Publicly reported outcomes

The reported scale changed quickly as the program expanded:

- In May 2025, BBVA said it had expanded to 11,000 licenses, with 83% of licensed users active daily and an average self-reported saving of 2.8 hours per week.
- In December 2025, BBVA announced access for more than 120,000 employees and deeper joint work with OpenAI.
- By mid-2026, OpenAI and BBVA reported roughly 100,000 regular users, more than 20,000 GPTs created, and selected workflow improvements of up to 80%.
- BBVA reported more than 8,000 active use cases in April 2026, with a smaller subset considered strategically reusable.

The figures refer to different dates and populations. They should not be combined as if they came from one controlled measurement.

## Why this is a strong AI FDE case

BBVA shows how FDE work changes at enterprise scale. The deployment required stakeholder alignment, safe access, training, domain-led prototyping, workflow review, reusable components, and a path from individual productivity to customer-facing systems. The partner relationship also evolved based on field adoption, which is the kind of feedback loop that should influence product and platform priorities.

## What remains unproven

- Time savings are self-reported and may vary by role and task.
- License use and GPT creation are adoption signals, not direct measures of customer or financial value.
- Public pages describe selected successful workflows but do not publish a full failure rate or portfolio-level return.
- Customer-facing projects announced in late 2025 should be separated from features already proven in production.

## FDE role alignment

- **R1. Embedded discovery and trusted partnership**
- **R2. Scoping and end-to-end delivery ownership**
- **R3. Hands-on implementation and systems integration**
- **R4. AI workflow and human-control design**
- **R6. Security, governance, reliability, and cost**
- **R7. Adoption and measurable business impact**
- **R8. Reusable patterns and field feedback**

See the [OpenAI and Amazon FDE role framework](../../role-requirements.md).

## References

1. [OpenAI, BBVA puts AI at the core of banking](https://openai.com/index/bbva/)
2. [BBVA, initial enterprise agreement with OpenAI](https://www.bbva.com/en/innovation/bbva-steps-up-its-plans-in-artificial-intelligence-by-signing-an-agreement-with-openai/)
3. [BBVA, expansion to 11,000 ChatGPT Enterprise licenses](https://www.bbva.com/en/innovation/bbva-expands-its-agreement-with-openai-to-11000-chatgpt-licences-for-the-banks-employees/)
4. [BBVA, strategic alliance to redefine banking with AI](https://www.bbva.com/en/innovation/bbva-and-openai-seal-a-strategic-alliance-to-redefine-banking-with-artificial-intelligence/)
5. [BBVA, AI adoption through talent](https://www.bbva.com/en/innovation/bbva-drives-ai-adoption-through-talent/)
