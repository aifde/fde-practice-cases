# 01. Tampa General Hospital: AI care coordination built with forward-deployed engineers

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High |
| Deployment status | Production, expanded from one workflow in 2021 to more than a dozen by June 2024 |
| Customer | Tampa General Hospital (TGH) |
| Delivery partner | Palantir |
| AI surface | Patient placement, staffing, care coordination, sepsis workflows, and operational decision support |
| Why it is relevant to AI FDE | TGH and Palantir describe engineers working directly with clinical, operations, and analytics teams, shipping into live hospital workflows and measuring operational outcomes |

## Operational problem

Tampa General runs a large academic health system where patient placement, bed capacity, staffing, imaging, discharge, and acute-care decisions depend on information spread across clinical and operational systems. A model that only predicts risk does not solve this problem. The output has to reach the right team, at the right point in the workflow, with enough context for a safe decision.

TGH began working with Palantir in 2021. The early work connected operational data and supported patient-flow decisions. The partnership later expanded into an AI-enabled care-coordination platform. TGH says the system now supports more than 20 applications, called Tiles, inside its 24-hour Care Coordination Center.

## Delivery approach

The delivery model was workflow-first. Palantir engineers worked with TGH operations, analytics, and clinical subject-matter experts. The team did not start with a general hospital chatbot. It identified specific decisions such as where a patient should be placed, which discharge barrier needs attention, and which staffing action is required.

The technical platform combined real-time operational data, predictive analytics, and later Palantir AIP and large language models. TGH retained clinical ownership. The AI layer supplied prioritization, summaries, and decision support while hospital teams remained responsible for care decisions.

~~~mermaid
flowchart LR
  A[Clinical and operational systems] --> B[Shared patient and capacity model]
  B --> C[Predictive analytics and AI workflows]
  C --> D[Placement, staffing, discharge, and sepsis queues]
  D --> E[Clinical and operations review]
  E --> F[Action in the live care workflow]
  F --> G[Outcome and workflow feedback]
  G --> B
~~~

## System and human-control design

| Layer | What the public evidence shows |
| --- | --- |
| Data | Real-time patient-flow, capacity, staffing, and care data are brought into a shared operational view. |
| Decision support | Applications surface placement priorities, discharge barriers, imaging bottlenecks, staffing needs, and risk signals. |
| Human control | Clinical and operational teams review the information and remain accountable for patient-care decisions. |
| Rollout | The work moved from an initial use case to more than a dozen workflows, then to a broader care-coordination operating system. |
| Feedback | Operational results and frontline use informed further applications and workflow changes. |

This is important for FDE work because the hard part was not a single model endpoint. The team had to connect data, encode hospital-specific decision rules, fit the tools into a command center, and earn adoption from people working under clinical and operational pressure.

## Publicly reported outcomes

TGH reported the following results in June 2024:

- 83% less time required to place patients.
- A 28% reduction in post-anesthesia care unit holds.
- A 30% reduction in mean length of stay for sepsis patients.
- Expansion from one use case to more than a dozen across the health system.

TGH's current Care Coordination Center page reports a broader set of outcomes, including $40 million in system-wide cost savings, 20,000 excess hospital days eliminated, a 25% reduction in emergency-room diversions, and the equivalent of 30 additional beds without physical expansion.

These are TGH and Palantir disclosures. The public pages do not provide a complete experimental design, confidence intervals, or enough information to attribute every result solely to the AI platform.

## Why this is a strong AI FDE case

The case has the features that distinguish forward deployment from a software handoff:

1. Engineers worked with domain experts inside a high-stakes operating environment.
2. The team scoped around concrete decisions rather than a generic AI capability.
3. The product connected to live systems and existing operational routines.
4. Rollout depended on frontline adoption, not only technical completion.
5. The first deployment created reusable data and workflow foundations for later applications.

## What remains unproven

- The public evidence does not isolate the effect of AI from process redesign, staffing changes, or other technology in the Care Coordination Center.
- Detailed model evaluations, failure rates, alert precision, and subgroup performance are not public.
- Reported operational improvements come from the participating organizations rather than an independent clinical study.

## FDE role alignment

- **R1. Embedded discovery and trusted partnership**
- **R2. Scoping and end-to-end delivery ownership**
- **R3. Hands-on implementation and systems integration**
- **R5. Evaluation and production quality**
- **R6. Security, governance, reliability, and cost**
- **R7. Adoption and measurable business impact**
- **R8. Reusable patterns and field feedback**

See the [OpenAI and Amazon FDE role framework](../../role-requirements.md).

## References

1. [Tampa General Hospital, AI software for connected care coordination](https://www.tgh.org/news/tgh-press-releases/2024/june/tgh-selects-palantir-ai-software-connected-care-coordination)
2. [Tampa General Hospital, Care Coordination Center](https://www.tgh.org/about-tgh/care-coordination-center)
3. [Palantir, AI platforms for hospitals](https://www.palantir.com/offerings/palantir-for-hospitals/)
4. [Healthcare IT News, Tampa General's AI-enabled care coordination](https://www.healthcareitnews.com/news/tampa-generals-investment-ai-enabled-care-coordination-software-saves-nearly-600-lives)
