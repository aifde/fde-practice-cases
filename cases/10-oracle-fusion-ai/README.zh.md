# 10. Oracle 与 Cohere：嵌入 Fusion Applications 的 100 多个 AI 用例

[English](README.md) | 中文 | [日本語](README.ja.md)

| 项目 | 证据 |
| --- | --- |
| 置信度 | 产品集成和已发布功能证据高，业务影响多为定性描述 |
| 部署状态 | 通过 Oracle Fusion Cloud Applications 和季度更新进入生产 |
| 客户与平台方 | Oracle |
| 交付方 | Cohere |
| AI 场景 | ERP、人力资源、供应链、销售、营销、服务、搜索、检索、生成和代理工作流 |
| 与 AI FDE 的关系 | Cohere 与 Oracle 团队共同处理 100 多个用例，把现场需求转成共享检索、模型、安全和发布模式 |

## 业务问题

Oracle Fusion Applications 服务多个业务部门和 14,000 多家客户。在这种环境中加入生成式 AI 是一个项目组合问题：每项功能都需要正确业务上下文、稳定安全边界、合适模型行为，以及企业客户可以采用的发布路径。

如果每个团队各自做聊天机器人，检索、治理、评估和集成工作会重复。Oracle 需要共同架构，支持 ERP、HCM、供应链、销售、营销和服务中的大量小型工作流功能。

## 交付过程

Oracle 与 Cohere 组合 Command R、Command R+、Embed 和 Rerank。检索增强生成让回答基于企业信息，减少无依据内容；Embed 支持语义检索，Rerank 改善候选结果的顺序和相关性。

双方共同处理 100 多个生成式 AI 用例，包括财务叙事、项目摘要、供应商建议、谈判摘要、候选人助手、客服聊天摘要和营销内容辅助。这些功能嵌入现有 Fusion 页面，并通过 Oracle 常规季度更新交付。

~~~mermaid
flowchart LR
  A[ERP、HCM、SCM、销售、营销和服务数据] --> B[Oracle 应用上下文与权限]
  B --> C[Embed 与语义检索]
  C --> D[Rerank 与依据上下文]
  D --> E[Command 生成或代理工作流]
  E --> F[Fusion 内嵌功能]
  F --> G[业务用户复核与操作]
  G --> H[季度发布与项目组合反馈]
  H --> B
~~~

## 共享生产架构

| 要求 | 公开资料中的方法 |
| --- | --- |
| 依据 | RAG 把企业应用上下文与 Cohere 生成连接起来。 |
| 检索质量 | Embed 与 Rerank 改善语义搜索和结果排序。 |
| 数据边界 | 功能运行在 Oracle 应用和 OCI 安全模型内，客户掌握数据治理。 |
| 产品集成 | AI 出现在财务、人力、供应链、销售、营销和服务工作流中。 |
| 复用 | 共享模型和检索组件支持大量功能，而不是单一应用。 |
| 发布 | 功能通过 Fusion Applications 季度更新持续改善。 |

## 公开结果

Cohere 在 2024 年 9 月披露，Fusion Applications 已支持 100 多个生成式 AI 用例。Oracle 后续产品材料描述了数百项 AI 功能、100 多个生成式 AI 用例和 50 多个代理工作流。

公开资料提供大量功能示例，但受控业务指标较少。最强证据是已经发布的集成广度和 Oracle 产品文档中的具体功能，而不是某一个生产率百分比。

## 为什么属于高置信度 AI FDE 案例

这个案例展示了现场工程怎样演变成平台工程。团队把许多工作流要求整理成可复用架构、治理与发布机制，工作横跨模型、检索、安全、应用设计、客户数据边界和持续产品交付，最终成果不是一次概念验证，而是持久企业产品的一部分。

## 尚未证明的部分

- 用例数量不能证明每项功能都被采用或创造价值。
- 公开资料没有披露统一评估框架、逐功能错误率和客户级使用数据。
- 部分功能属于生成辅助，不是自主代理。
- 速度和准确性收益大多没有受控测量。

## FDE 岗位能力对应

- **R1. 嵌入式需求发现与可信协作**
- **R2. 范围界定与端到端交付**
- **R3. 亲自实现与系统集成**
- **R4. AI 工作流与人工控制设计**
- **R5. 评估与生产质量**
- **R6. 安全、治理、可靠性与成本**
- **R7. 采用与可量化业务影响**
- **R8. 可复用资产与现场反馈**

参见 [OpenAI 与 Amazon FDE 岗位能力框架](../../role-requirements.zh.md)。

## 引用来源

1. [Cohere，Oracle 客户案例](https://cohere.com/customer-stories/oracle)
2. [Oracle，AI for Fusion Applications](https://www.oracle.com/pe/a/ocom/docs/applications/oracle-ai-for-fusion-apps.pdf)
3. [Cohere，Oracle 生成式 AI 服务公告](https://cohere.com/blog/oracle-to-deliver-powerful-and-secure-generative-ai-services-for-business)
4. [Cohere，Oracle Cloud Infrastructure 企业 AI](https://cohere.com/blog/generative-ai-service-ga)
