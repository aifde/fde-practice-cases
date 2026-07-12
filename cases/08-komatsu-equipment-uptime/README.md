# 08. Komatsu：矿山设备服务与停机时间

[来源：Palantir Master Classes](https://www.palantir.com/master-classes/)

~~~mermaid
flowchart LR
  A[设备遥测与服务记录] --> B[资产健康语义层]
  B --> C[故障与服务优先级]
  C --> D[现场服务团队]
~~~

**问题与交付。** 重型设备的停机影响产能，服务人员需要把遥测、维护历史和客户现场状态放在一起判断。Komatsu 将 Foundry/AIP 用于提升服务效率和设备可用性。

**公开成果与 FDE 启示。** 公开访谈强调快速改善运营卓越性。FDE 切入点不是泛化预测性维护，而是先选一个高价值的“服务何时介入”决策，绑定停机时长、首次修复率和技术员采纳率。

中文 | [English](README.en.md) | [日本語](README.ja.md)
