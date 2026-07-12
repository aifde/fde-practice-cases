# 18. Klarna：把多语言客服代理接进退款与退货流程

[来源：OpenAI Klarna 案例](https://openai.com/index/klarna/)

~~~mermaid
flowchart LR
  A[客户对话和订单状态] --> B[多语言 AI 助手]
  B --> C[退款退货与转人工]
  C --> D[客户完成事项]
~~~

**问题与交付。** 客服代理必须理解订单、退款和退货状态，而不仅是回答 FAQ。Klarna 把 AI 助手纳入这些交易流程，并在多市场、多语言环境下运行。

**公开成果与 FDE 启示。** OpenAI 披露首月完成 230 万次对话、重复咨询下降 25%、处理时长由 11 分钟降至不足 2 分钟。可复用方法是优先把代理接入可验证的后端动作，同时保持对例外情形的人工升级。

中文 | [English](README.en.md) | [日本語](README.ja.md)
