# 09. Draftwise and Cohere: source-grounded AI for contract drafting

English | [中文](README.zh.md) | [日本語](README.ja.md)

| Field | Evidence |
| --- | --- |
| Confidence | High for the product integration; performance figures come from internal benchmarks |
| Deployment status | Production product used for legal drafting and retrieval |
| Customer | Draftwise |
| Delivery partners | Cohere and Microsoft Azure AI Foundry |
| AI surface | Contract search, retrieval-augmented generation, clause suggestions, citations, and drafting support |
| Why it is relevant to AI FDE | The team started from lawyer workflows, combined several models into a production retrieval stack, and treated source traceability and security as product requirements |

## Operational problem

Lawyers drafting and negotiating contracts need to find relevant language across prior agreements, communications, and client documents. Keyword search often misses semantically similar clauses, while unconstrained generation can produce language that is difficult to verify. A legal AI system must help users locate precedent and show where a suggestion came from.

Draftwise's product goal was not to replace legal judgment. It was to reduce repetitive searching and drafting while keeping customer expertise and source documents visible to the lawyer.

## Delivery approach

The Draftwise team interviewed prospective customers to understand how lawyers search, draft, and review agreements. It then built Smart Draft as a retrieval-augmented generation system using Cohere models through Azure AI Foundry.

The stack assigned different work to different models:

- Cohere Embed represented contracts and other material by semantic meaning.
- Cohere Rerank reordered retrieved material so the most relevant examples appeared first.
- Cohere Command generated drafting assistance and cited source documents.
- Fine-tuning adapted model behavior to the product's legal search requirements.

~~~mermaid
flowchart LR
  A[Prior contracts and client documents] --> B[Document processing and embeddings]
  B --> C[Semantic retrieval]
  C --> D[Cohere Rerank]
  D --> E[Grounded generation with citations]
  E --> F[Lawyer review and editing]
  F --> G[Approved contract language]
  F --> H[Failed-search and quality feedback]
  H --> C
~~~

## Evaluation and control design

The public case emphasizes search-result quality rather than a general language-model benchmark. That is the correct unit for the product: a lawyer cannot review a useful clause if retrieval never surfaces it.

Traceable citations are a second control. They allow a user to inspect the source agreement rather than trust a generated clause on appearance. Azure deployment was selected partly because the founders and customers already trusted the surrounding enterprise environment.

A production legal workflow still requires controls that are not fully described publicly, including matter-level access, ethical walls, document retention, privilege protection, and version history. The case shows the retrieval and generation design, but not the entire law-firm governance model.

## Publicly reported outcomes

Cohere and Draftwise report:

- A 30% improvement in search-result quality on Draftwise internal benchmarks after incorporating fine-tuned Cohere models.
- A threefold increase in model API calls during the first quarter of 2025.
- Faster access to relevant clauses and examples from past agreements.

The first metric is directly relevant to the system but lacks a published dataset, baseline, or statistical analysis. API growth is an adoption signal, not proof of legal quality or time saved.

## Why this is a strong AI FDE case

The delivery began with domain interviews and a specific professional workflow. The architecture combined generation, embeddings, reranking, citations, and secure cloud deployment. It also placed the lawyer at the final decision point. This is the kind of multi-layer implementation expected from an FDE: model selection is only one part of the work.

## What remains unproven

- The internal search benchmark and grading method are not public.
- No public study measures drafting time, error rates, negotiation outcomes, or client value.
- The case does not disclose how permissions and legal ethical walls are enforced.
- Increased API usage may reflect customer growth, feature expansion, or heavier usage and should not be treated as a quality metric.

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

1. [Cohere, Draftwise customer story](https://cohere.com/customer-stories/draftwise)
2. [Cohere, legal work with AI and the Draftwise story](https://cohere.com/blog/legal-work-with-ai-the-draftwise-story)
3. [Draftwise, Smart Draft](https://www.draftwise.com/)
