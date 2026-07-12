# 02. NHS Federated Data Platform：把患者流转做成可执行工作流

~~~mermaid
flowchart LR
  A[电子病历与社护数据] --> B[本地 FDP 实例]
  B --> C[等候名单和出院产品]
  C --> D[临床与运营团队协作]
~~~

**问题与交付。** 医院、社护和预约系统数据分散，使出院和等候名单管理依赖人工追问。FDP 将既有运营数据连接到本地实例，再以等待名单验证、OPTICA 出院规划等具体产品进入团队日常工作。

**公开成果与 FDE 启示。** NHS 截至 2026 年 5 月披露 139 家信托已上线；OPTICA 的长住患者延迟天数在前后 12 个月对比中下降。可复用方法是以单一临床路径切入，同时配置数据治理、实施负责人、桌边培训和持续收益度量。

## 引用来源

1. [来源：NHS England FDP 成效数据](https://www.england.nhs.uk/digitaltechnology/nhs-federated-data-platform/impact/fdp-uptake-and-benefits/)

中文 | [English](README.en.md) | [日本語](README.ja.md)
