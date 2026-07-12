# 29. Notion：工作区搜索的精准重排

[来源：Cohere Notion 案例](https://cohere.com/fr/customer-stories/notion)

~~~mermaid
flowchart LR
  A[Notion、Slack 和 Drive 内容] --> B[候选检索]
  B --> C[重排与生成回答]
  C --> D[多语言团队使用]
~~~

**问题与交付。** 组织知识分布在工作区和连接器中，先召回再回答容易让不相关内容污染上下文。Notion 在搜索管线中加入重排，并以可扩缩云基础设施支撑不同规模的工作区。

**公开成果与 FDE 启示。** 案例强调以精准度、成本和多语言体验为共同目标。可复用方法是按工作区规模设计不同检索路径，并用真实失败查询持续校正召回与重排。

中文 | [English](README.en.md) | [日本語](README.ja.md)
