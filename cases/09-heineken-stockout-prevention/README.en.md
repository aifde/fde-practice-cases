# 09. Heineken USA: distributor stockout prevention

~~~mermaid
flowchart LR
  A[Brewery, warehouse, and distributor data] --> B[Live supply-chain view]
  B --> C[Stockout risk and schedule changes]
  C --> D[Supply-chain execution]
~~~

**Delivery.** The deployment joins production, warehouse, customer, and vessel data to identify disruptions early and adjust delivery plans.

**FDE lesson.** Launch with a replayable exception queue. Palantir reports that 25 distributor alerts worth about $300,000 were resolved in two test days, then expand only after alerts change real dispatch choices.

## References

1. [Source: Palantir Impact](https://www.palantir.com/impact/)

[中文](README.md) | English | [日本語](README.ja.md)
