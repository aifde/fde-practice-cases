# 03. Morgan Stanley: evaluation-first AI for regulated wealth management

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High |
| Deployment status | Production, with firmwide wealth-management rollout |
| Customer | Morgan Stanley Wealth Management |
| Delivery partner | OpenAI |
| AI surface | Internal knowledge retrieval, research summarization, meeting notes, follow-up drafts, and CRM writeback |
| Why it is relevant to AI FDE | Customer and model teams built representative evaluations, retrieval methods, controls, and workflow integrations before scaling adoption |

## Operational problem

Financial advisors need fast access to a large body of approved research and internal knowledge. A plausible but unsupported answer is unacceptable in a regulated environment. Meeting summaries create a second challenge: the system must capture actions accurately, respect client consent, and keep the advisor responsible for the final record and communication.

Morgan Stanley and OpenAI therefore treated evaluation as part of the product, not as a final benchmark. The deployment began with narrow goals: improve information retrieval, summarize approved material, and support advisor preparation without removing professional judgment.

## Delivery approach

For AI @ Morgan Stanley Assistant, the team tested model behavior against real advisor questions and used expert graders to assess accuracy and coherence. As the document corpus grew, Morgan Stanley and OpenAI refined retrieval methods and expanded the evaluation set. The public case says the system moved from answering about 7,000 questions to supporting questions over a corpus of 100,000 documents.

The next product, AI @ Morgan Stanley Debrief, turns consented meeting recordings into notes, action items, and a draft follow-up. Advisors review the output before it is sent or finalized. Notes can then be saved into Salesforce, which places AI inside the existing advisor workflow rather than in a separate experiment.

~~~mermaid
flowchart LR
  A[Approved research and internal documents] --> B[Retrieval pipeline]
  B --> C[Assistant response]
  D[Consented meeting recording] --> E[Transcription and summarization]
  E --> F[Notes, actions, and draft follow-up]
  C --> G[Advisor review]
  F --> G
  G --> H[Client conversation or CRM record]
  H --> I[Expert feedback and regression cases]
  I --> B
  I --> E
~~~

## Evaluation and governance

The public material describes several layers of control:

- Advisors and prompt engineers graded answers using real questions.
- Summarization evaluations measured whether key information was preserved without adding errors.
- Translation evaluations were added for multilingual client needs.
- Debrief used datasets representing different meeting types and tested action-item capture.
- A daily regression suite checked sample questions for quality and compliance weaknesses.
- Advisors retained final approval over notes and communications.
- Morgan Stanley cited zero data retention as an important security condition for the relationship.

These controls show why enterprise evaluation is more than a single accuracy score. It includes representative data, professional judgment, regression testing, retrieval quality, consent, and workflow authority.

## Publicly reported outcomes

OpenAI and Morgan Stanley report:

- More than 98% adoption among financial-advisor teams.
- Growth in accessible documents from about 20% to 80%.
- Expansion from the Assistant to Debrief and additional planned use cases.
- Follow-up work that previously took days moving to hours in reported advisor experience.

Morgan Stanley independently confirmed the 98% adoption figure when it announced Debrief in June 2024.

## Why this is a strong AI FDE case

The deployment joined customer discovery, regulated knowledge, retrieval engineering, evaluation, security, user consent, human review, and CRM integration. It also created reusable evaluation assets that supported more than one application. Field feedback affected retrieval methods and the product roadmap, matching the feedback loop expected from a mature FDE engagement.

## What remains unproven

- The detailed evaluation datasets, graders, thresholds, and error rates are not public.
- Adoption does not by itself prove investment returns or better client outcomes.
- Most performance claims come from the participating organizations.
- The effect of AI is difficult to separate from training, workflow redesign, and broader platform improvements.

## FDE role alignment

- **R1. Embedded discovery and trusted partnership**
- **R3. Hands-on implementation and systems integration**
- **R4. AI workflow and human-control design**
- **R5. Evaluation and production quality**
- **R6. Security, governance, reliability, and cost**
- **R7. Adoption and measurable business impact**
- **R8. Reusable patterns and field feedback**

See the [OpenAI and Amazon FDE role framework](../../role-requirements.md).

## References

1. [OpenAI, Morgan Stanley uses AI evals to shape financial services](https://openai.com/index/morgan-stanley/)
2. [Morgan Stanley, launch of AI @ Morgan Stanley Debrief](https://www.morganstanley.com/press-releases/ai-at-morgan-stanley-debrief-launch)
3. [Morgan Stanley, Insights and Outcomes, Volume 6](https://www.morganstanley.com/cs/pdf/FOR-Insights-and-Outcomes-VOL6-layout-ebook-digital.pdf)
