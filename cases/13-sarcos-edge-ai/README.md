# 13. Sarcos：机器人与边缘 AI 的现场协同

[来源：Palantir Foundry 工程制造案例](https://www.palantir.com/platforms/foundry/)

~~~mermaid
flowchart LR
  A[机器人运行与任务数据] --> B[边缘 AI 操作系统]
  B --> C[任务与性能洞察]
  C --> D[现场操作员和工程师]
~~~

**问题与交付。** 机器人系统只有与任务现场、设备状态和维护节奏连接，才会成为生产能力。公开材料描述 Sarcos 把机器人能力与边缘 AI 操作系统结合。

**公开成果与 FDE 启示。** 可复用方法是把现场网络、故障降级和人工接管当作核心产品需求；在真实场地先验证少量任务，而非从云端指标推断可用性。

中文 | [English](README.en.md) | [日本語](README.ja.md)
