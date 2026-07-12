# 18. Klarna: multilingual support connected to refunds and returns

~~~mermaid
flowchart LR
  A[Customer conversation and order state] --> B[Multilingual AI assistant]
  B --> C[Refund, return, or handoff]
  C --> D[Customer resolution]
~~~

**Delivery.** Klarna integrated an AI assistant with the support workflows that involve order information, refunds, and returns, rather than limiting it to static FAQs.

**FDE lesson.** Connect an agent to verifiable back-end actions and define human escalation for exceptions. OpenAI reports 2.3 million conversations in the first month, a 25% fall in repeat inquiries, and completion in under two minutes versus 11 minutes.

## References

1. [Source: OpenAI, Klarna](https://openai.com/index/klarna/)

[中文](README.md) | English | [日本語](README.ja.md)
