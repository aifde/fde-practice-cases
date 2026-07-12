# 10. Wendy's QSCC: inventory balancing across a restaurant network

~~~mermaid
flowchart LR
  A[Orders, inventory, and DC data] --> B[Restaurant supply model]
  B --> C[Shortage and reallocation choices]
  C --> D[Operations approval]
~~~

**Delivery.** Wendy's QSCC tracks orders and inventory across a large restaurant network, models distribution-center needs, and supports resource reallocation.

**FDE lesson.** Build decision rights into the system. A shortage forecast needs an owner, an escalation path, and an explanation of the operational tradeoff before it can become an automated action.

## References

1. [Source: Palantir Impact](https://www.palantir.com/impact/)

[中文](README.md) | English | [日本語](README.ja.md)
