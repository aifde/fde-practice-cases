# 08. CoreWeave and Cohere: an on-site workshop to a production support agent in 90 days

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High, with a detailed named workflow and production timeline; metrics are participant-reported |
| Deployment status | Broad production deployment after 90 days |
| Customer | CoreWeave |
| Delivery partner | Cohere solutions architects |
| AI surface | Slack-based support intake, context gathering, routing, engineering swarming, and resolution assistance |
| Why it is relevant to AI FDE | The engagement began with a two-day on-site workflow mapping session and ended with a privately deployed agent integrated into CoreWeave's real support systems |

## Operational problem

CoreWeave's support model connects customers directly with engineers. As demand grew, support engineers had to collect missing context, move between Slack and ticketing tools, create issues, find the correct engineering team, and search past documentation and post-ticket reviews. The process was slow because the information path was fragmented, not because support engineers lacked technical expertise.

The delivery target was therefore precise: reduce intake and routing friction without replacing expert engineering judgment or forcing customers and engineers into a new chat product.

## Delivery approach

Cohere began with a two-day on-site session involving CoreWeave engineering and business teams. The group mapped the entire support process, identified the specialized knowledge agents would need, selected integration points, and established a delivery timeline.

The team embedded Cohere North into Slack, CoreWeave's existing support channel. North was privately deployed in CoreWeave data centers so sensitive customer data stayed inside the security perimeter. The architecture allowed CoreWeave to choose models and configurations for different steps.

~~~mermaid
flowchart LR
  A[Customer issue in Slack] --> B[North triage agent]
  B --> C[Region, cluster, and account context]
  C --> D[Support engineer review]
  D --> E[Jira issue and engineering swarming channel]
  E --> F[North resolution agent]
  F --> G[Documentation and historical ticket reviews]
  G --> H[Engineer diagnosis and customer resolution]
  H --> I[Post-ticket feedback]
  I --> F
~~~

## Production workflow

The public case describes the flow in detail:

1. A support issue arrives through Slack.
2. A customer-support engineer triggers the triage bot.
3. North gathers customer context such as region and cluster from backend systems.
4. The engineer checks the intake information and adds nuance.
5. Automation creates a Jira issue and opens a swarming channel with relevant engineering teams.
6. A resolution agent retrieves documentation and historical post-ticket reviews.
7. Engineers use the suggested context and resolution material to solve the issue.

Human review remains in two critical places: confirmation of ticket context and final technical resolution. The agent reduces assembly work but does not silently act on customer infrastructure.

## Publicly reported outcomes

Cohere and CoreWeave reported:

- Broad production deployment within 90 days.
- Mean resolution time reduced from four to eight days to two to five days.
- Customer-satisfaction scores of 4.9 to 5.0 for the large majority of tickets during the first months.
- Higher routing accuracy and fewer manual steps.
- Change management and internal training completed within one business week.

The published article attributes the outcome to improved internal procedures together with North automation. That wording matters because the effect should not be assigned to the model alone.

## Security and reliability considerations

Private deployment kept customer data within CoreWeave's perimeter. CoreWeave's separate support-access documentation also describes time-bound, auditable employee access and customer approval for access to managed environments. The public case does not state that North itself requested this privileged access, but the surrounding control model shows why support automation must respect existing identity and audit boundaries.

## Why this is a strong AI FDE case

This is the clearest forward-deployment pattern in the library: an on-site workshop, joint workflow mapping, explicit success measures, integration with existing systems, private deployment, rapid production rollout, human control, and a plan to reuse the pattern for incident response. The team removed workflow friction before attempting broader automation.

## What remains unproven

- Metrics come from a Cohere customer story and are not independently audited.
- The article does not publish ticket mix, severity distribution, or a controlled before-and-after analysis.
- The relative contribution of process redesign and model automation is not isolated.
- Longer-term drift, cost, and reliability data are not public.

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

1. [Cohere, CoreWeave customer-support case study](https://cohere.com/customer-stories/coreweave)
2. [CoreWeave, support access management](https://docs.coreweave.com/changelog/release-notes/support-access-management)
3. [CoreWeave, Cohere infrastructure case study](https://www.coreweave.com/resources/case-studies/cohere-accelerates-training-of-north-agentic-ai-for-enterprise)
