# 10. Oracle and Cohere: more than 100 AI use cases embedded in Fusion Applications

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High for the product integration and released feature portfolio; business-impact figures are mostly qualitative |
| Deployment status | Production features delivered through Oracle Fusion Cloud Applications and quarterly updates |
| Customer and platform owner | Oracle |
| Delivery partner | Cohere |
| AI surface | ERP, HR, supply chain, sales, marketing, service, search, retrieval, generation, and embedded agent workflows |
| Why it is relevant to AI FDE | Cohere and Oracle teams worked across more than 100 use cases, turning field requirements into shared retrieval, model, security, and release patterns inside an enterprise suite |

## Operational problem

Oracle Fusion Applications serves many business functions and more than 14,000 customers. Adding generative AI to this environment creates a portfolio problem. Each feature needs access to the correct business context, predictable security and data boundaries, suitable model behavior, and a release path that enterprise customers can adopt.

A collection of disconnected chatbots would duplicate retrieval, governance, evaluation, and integration work. Oracle needed a common architecture that could support many small workflow features across ERP, HCM, supply chain, sales, marketing, and service.

## Delivery approach

Oracle and Cohere combined Command R and Command R+ with Embed and Rerank. Retrieval-augmented generation grounded responses in enterprise information and reduced unsupported output. Embed supported semantic retrieval, while Rerank improved the order and relevance of candidate results.

The teams worked across more than 100 generative-AI use cases. Examples include financial narrative generation, project summaries, supplier recommendations, negotiation summaries, candidate assistants, service-chat summaries, and sales or marketing authoring. The features were embedded in existing Fusion screens and shipped through Oracle's regular quarterly update process.

~~~mermaid
flowchart LR
  A[ERP, HCM, SCM, sales, marketing, and service data] --> B[Oracle application context and permissions]
  B --> C[Embed and semantic retrieval]
  C --> D[Rerank and grounded context]
  D --> E[Command generation or agent workflow]
  E --> F[Embedded Fusion application feature]
  F --> G[Business-user review and action]
  G --> H[Quarterly release and portfolio feedback]
  H --> B
~~~

## Shared production architecture

| Requirement | Publicly described approach |
| --- | --- |
| Grounding | RAG combines enterprise application context with Cohere generation. |
| Retrieval quality | Embed and Rerank improve semantic search and result ordering. |
| Data boundaries | Features run within Oracle's application and OCI security model, with customer control over data governance. |
| Product integration | AI appears inside finance, HR, supply-chain, sales, marketing, and service workflows. |
| Reuse | Shared models and retrieval components support a large portfolio rather than one custom application. |
| Release | Features improve through Fusion Applications' quarterly updates. |

## Publicly reported outcomes

Cohere's September 2024 customer story reported more than 100 generative-AI use cases supported across Fusion Applications. Oracle's later product material describes hundreds of AI features, more than 100 generative-AI use cases, and more than 50 agentic workflows.

The public sources provide many feature examples but few controlled business-outcome measurements. The strongest evidence is breadth of released integration and the presence of the features in Oracle product documentation, not a single productivity percentage.

## Why this is a strong AI FDE case

This case shows how field engineering becomes platform engineering. Teams had to convert many workflow requirements into reusable architecture, governance, and release mechanisms. The work crossed model selection, retrieval, security, application design, customer data boundaries, and ongoing product delivery. The result was not a one-off proof of concept. It became part of a durable enterprise product surface.

## What remains unproven

- A use-case count does not show adoption or value for every feature.
- Public materials do not disclose a common evaluation framework, per-feature error rates, or customer-level usage.
- Some listed capabilities are generative features rather than autonomous agents.
- Benefits such as improved speed and accuracy are generally described without controlled measurements.

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

1. [Cohere, Oracle customer story](https://cohere.com/customer-stories/oracle)
2. [Oracle, AI for Fusion Applications](https://www.oracle.com/pe/a/ocom/docs/applications/oracle-ai-for-fusion-apps.pdf)
3. [Cohere, Oracle generative-AI services announcement](https://cohere.com/blog/oracle-to-deliver-powerful-and-secure-generative-ai-services-for-business)
4. [Cohere, enterprise AI on Oracle Cloud Infrastructure](https://cohere.com/blog/generative-ai-service-ga)
