# 29. Notion: precision reranking for workspace search

~~~mermaid
flowchart LR
  A[Notion, Slack, and Drive content] --> B[Candidate retrieval]
  B --> C[Reranking and answer generation]
  C --> D[Multilingual teams]
~~~

**Delivery.** Notion introduced reranking into a search pipeline that reaches across workspaces and connected tools, with cloud scaling for variable demand.

**FDE lesson.** Design different retrieval paths for different workspace sizes, then improve recall and ranking with real failed searches. The case frames precision, cost, and multilingual experience as joint goals.

## References

1. [Source: Cohere, Notion](https://cohere.com/fr/customer-stories/notion)

[中文](README.md) | English | [日本語](README.ja.md)
