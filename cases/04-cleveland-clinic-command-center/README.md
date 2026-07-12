# 04. Cleveland Clinic：虚拟指挥中心优化医院资源

~~~mermaid
flowchart LR
  A[床位、手术室和出院信号] --> B[虚拟指挥中心]
  B --> C[资源与人员配置建议]
  C --> D[运营负责人执行]
~~~

**问题与交付。** 床位分配、出院、手术室时段和人员配置相互牵连，单个科室的局部优化会制造全局堵点。虚拟指挥中心把这些资源放进同一运营视图，由负责人对建议进行取舍。

**公开成果与 FDE 启示。** 公开材料将其用途列为缩短等待、改善住院时长、平衡人员配置和提高关键资源利用。FDE 应把“谁能改变什么”固化为权限和例会机制，不能只交付分析。

## 引用来源

1. [来源：Palantir Foundry 医疗交付案例](https://www.palantir.com/platforms/foundry/)

中文 | [English](README.en.md) | [日本語](README.ja.md)
