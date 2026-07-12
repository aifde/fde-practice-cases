# 05. Moderna: enterprise AI adoption with clinical judgment kept in the loop

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High for deployment and adoption; moderate for detailed clinical-performance claims |
| Deployment status | Production enterprise rollout with continuing expansion |
| Customer | Moderna |
| Delivery partner | OpenAI |
| AI surface | Internal assistants across research, legal, manufacturing, commercial work, protocol writing, regulatory documents, and clinical analysis support |
| Why it is relevant to AI FDE | The program combined internal APIs, enterprise rollout, domain-led assistants, change management, and explicit human ownership in a high-stakes industry |

## Operational problem

Moderna operates across scientific research, clinical development, manufacturing, legal, regulatory, and commercial functions. A general assistant can help with routine work, but clinical and regulatory workflows require traceable evidence and clear professional accountability. Scaling AI across those functions also requires more than issuing licenses. Employees need training, usable internal patterns, and a way to build assistants around domain-specific work.

## Delivery approach

Moderna began working with OpenAI in early 2023. It first built mChat on the OpenAI API, then deployed ChatGPT Enterprise across business functions. Moderna paired the technology rollout with listening sessions, training, office hours, internal forums, leadership participation, and a network of generative-AI champions.

Employees created task-specific GPTs for legal, research, manufacturing, marketing, and sales. One published example, Dose ID, supports a clinical study team evaluating vaccine dose selection. The tool applies standard criteria, cites sources, explains its rationale, and produces visualizations. The clinical team retains the decision.

~~~mermaid
flowchart LR
  A[Approved enterprise data and documents] --> B[mChat, ChatGPT Enterprise, and custom GPTs]
  B --> C[Domain-specific analysis or draft]
  C --> D[Sources, rationale, and visual output]
  D --> E[Scientist, clinician, legal, or business review]
  E --> F[Approved workflow decision or document]
  F --> G[Training, feedback, and reusable GPT patterns]
  G --> B
~~~

## Adoption and human-control design

Moderna's public material emphasizes people and operating structure:

- mChat reached more than 80% employee use before the wider enterprise rollout.
- Champions and office hours helped teams move from prompting practice to work-specific assistants.
- Executives participated in the change program rather than treating adoption as an IT project.
- High-stakes outputs were positioned as decision support, with domain experts retaining approval.
- GPTs were distributed across many functions instead of being concentrated in one innovation team.

This is an FDE-relevant pattern because domain experts were not only end users. They helped define the problems, build assistants, review outputs, and spread successful practices.

## Publicly reported outcomes

Moderna and OpenAI reported more than 750 custom GPTs within the first months of ChatGPT Enterprise deployment. Moderna's 2025 shareholder letter later said the company had created more than 4,000 GPTs and was using the collaboration to support protocol writing, regulatory documents, trial design, data analysis, forecasting, and internal workflows.

The growth from hundreds to thousands of GPTs demonstrates adoption and experimentation. It does not establish that every GPT is active, safe, or valuable. The most useful evidence comes from named workflows, such as Dose ID, where the decision boundary and source requirements are described.

## Why this is a strong AI FDE case

The case connects technical deployment with domain ownership and change management. It also shows a sensible boundary for high-stakes AI: the system gathers, explains, and visualizes information, while qualified people make the clinical decision. The reusable asset is not only a model configuration. It includes training, champion networks, internal delivery practices, and patterns for source-grounded assistants.

## What remains unproven

- Public sources do not disclose Dose ID's evaluation dataset, error rates, validation thresholds, or effect on trial outcomes.
- The number of GPTs is an activity measure, not a portfolio-level quality measure.
- Productivity and scientific-impact claims are mostly qualitative.
- Clinical support examples should not be interpreted as autonomous diagnosis or treatment selection.

## FDE role alignment

- **R1. Embedded discovery and trusted partnership**
- **R2. Scoping and end-to-end delivery ownership**
- **R4. AI workflow and human-control design**
- **R5. Evaluation and production quality**
- **R6. Security, governance, reliability, and cost**
- **R7. Adoption and measurable business impact**
- **R8. Reusable patterns and field feedback**

See the [OpenAI and Amazon FDE role framework](../../role-requirements.md).

## References

1. [OpenAI, Moderna case study](https://openai.com/index/moderna/)
2. [Moderna, collaboration with OpenAI](https://www.modernatx.com/media-center/all-media/blogs/collaboration-with-openai)
3. [Moderna, 2025 shareholder letter](https://www.modernatx.com/media-center/all-media/blogs/moderna-2025-shareholder-letter)
4. [Moderna Japan, collaboration announcement and Dose ID example](https://www.modernatx.com/ja-JP/press-release/2024/20240501)
