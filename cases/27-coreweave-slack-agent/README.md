# 27. CoreWeave：90 天内把代理嵌入 Slack 支持链路

~~~mermaid
flowchart LR
  A[Slack 支持请求] --> B[分流代理补全上下文]
  B --> C[Jira 和专家协作频道]
  C --> D[解决代理给出建议]
~~~

**问题与交付。** 云基础设施支持需要快速把客户问题送到正确工程师，原流程跨越多个工具且缺少上下文。CoreWeave 与解决方案架构师先梳理端到端流程，再把代理放进已有 Slack 工作方式。

**公开成果与 FDE 启示。** 案例披露 90 天内投入生产、平均解决时间由 4 至 8 天降为 2 至 5 天。可复用方法是通过现场工作坊先消除手工断点，再选最少侵入的集成路径。

## 引用来源

1. [来源：Cohere CoreWeave 案例](https://cohere.com/customer-stories/coreweave)

中文 | [English](README.en.md) | [日本語](README.ja.md)
