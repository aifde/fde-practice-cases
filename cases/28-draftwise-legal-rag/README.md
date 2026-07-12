# 28. Draftwise：合同起草中的可追溯检索

~~~mermaid
flowchart LR
  A[历史合同和条款] --> B[语义检索与重排]
  B --> C[带来源的起草建议]
  C --> D[律师审核与谈判]
~~~

**问题与交付。** 律师需要从既有合同中找到准确的条款和先例，错误检索会直接降低对 AI 的信任。Draftwise 将生成、嵌入和重排模型组合为带引用的 RAG 工作流。

**公开成果与 FDE 启示。** 发布方称内部基准的搜索结果质量提升 30%。可复用方法是把“可回到原文”的证据链作为默认 UX，并让专业人员验证检索质量而非只评价文笔。

## 引用来源

1. [来源：Cohere Draftwise 案例](https://cohere.com/customer-stories/draftwise)

中文 | [English](README.en.md) | [日本語](README.ja.md)
