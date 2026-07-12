# 01. Tampa General Hospital：FDE 深度参与的医院 AI 协同系统

[English](README.md) | 中文 | [日本語](README.ja.md)

| 项目 | 证据 |
| --- | --- |
| 置信度 | 高 |
| 部署状态 | 已进入生产，从 2021 年的首个工作流扩展到 2024 年 6 月的十多个工作流 |
| 客户 | Tampa General Hospital（TGH） |
| 交付方 | Palantir |
| AI 场景 | 患者床位安排、人力调度、诊疗协同、脓毒症流程和运营决策支持 |
| 与 AI FDE 的关系 | TGH 与 Palantir 公开说明，工程师直接与临床、运营和分析团队合作，把系统部署进真实医院工作流并衡量运营结果 |

## 业务问题

Tampa General 运营着大型学术医疗体系。患者安置、床位容量、人力安排、影像检查、出院和急症决策依赖多个临床与运营系统中的信息。只给出风险分数的模型不能解决这个问题。结果必须在正确的时点送到正确的团队，并提供足够的上下文，让医护人员安全地作出决定。

TGH 从 2021 年开始与 Palantir 合作。早期工作连接运营数据并支持患者流转，随后扩展为 AI 驱动的诊疗协同平台。TGH 表示，其全天候运行的 Care Coordination Center 已经使用 20 多个应用，内部称为 Tiles。

## 交付过程

团队先处理工作流，而不是先做一个通用医院聊天机器人。Palantir 工程师与 TGH 的运营、分析和临床专家共同识别具体决策，例如患者应该安排到哪里、哪个出院障碍需要处理，以及当班人力需要怎样调整。

技术平台连接实时运营数据、预测分析、Palantir AIP 和大语言模型。TGH 仍然掌握临床决策权。AI 提供优先级、摘要和决策支持，医护与运营团队负责最终决定。

~~~mermaid
flowchart LR
  A[临床与运营系统] --> B[统一的患者与容量模型]
  B --> C[预测分析与 AI 工作流]
  C --> D[床位、人力、出院与脓毒症队列]
  D --> E[临床和运营人员复核]
  E --> F[在真实诊疗流程中执行]
  F --> G[结果与工作流反馈]
  G --> B
~~~

## 系统与人工控制

| 层面 | 公开资料能够证明的设计 |
| --- | --- |
| 数据 | 实时患者流转、容量、人力和诊疗数据进入统一运营视图。 |
| 决策支持 | 应用展示床位优先级、出院障碍、影像瓶颈、人力需求和风险信号。 |
| 人工控制 | 临床和运营团队复核信息，并对患者诊疗决定负责。 |
| 推广 | 项目从单个用例扩展到十多个工作流，再演变成诊疗协同操作系统。 |
| 反馈 | 一线使用和运营结果继续推动后续应用和流程调整。 |

这个案例的难点不在一个模型接口，而在于连接数据、编码医院特有规则、把工具接入指挥中心，并让高压环境下的一线人员真正使用。

## 公开结果

TGH 在 2024 年 6 月披露：

- 患者安置所需时间减少 83%。
- 麻醉后监护区滞留减少 28%。
- 脓毒症患者平均住院时长减少 30%。
- 从一个用例扩展到全院十多个工作流。

TGH 当前的 Care Coordination Center 页面还披露了更大范围的结果：全系统节省 4,000 万美元、减少 20,000 个额外住院日、急诊分流减少 25%，并在不扩建的情况下获得相当于 30 张床位的容量。

这些数字来自 TGH 与 Palantir。公开页面没有提供完整实验设计、置信区间，也不足以把所有结果单独归因于 AI 平台。

## 为什么属于高置信度 AI FDE 案例

1. 工程师进入高风险现场，与领域专家共同工作。
2. 项目围绕具体决策，而不是通用 AI 能力划定范围。
3. 产品连接生产系统并进入现有运营流程。
4. 是否成功取决于一线采用和运营结果，不只是代码上线。
5. 首个项目留下可供后续应用复用的数据和工作流底座。

## 尚未证明的部分

- 公开资料无法分离 AI、流程重构、人力变化和指挥中心其他技术的各自贡献。
- 模型评估、失败率、预警精度和不同患者群体的表现没有公开。
- 运营结果来自参与机构，并非独立临床研究。

## FDE 岗位能力对应

- **R1. 嵌入式需求发现与可信协作**
- **R2. 范围界定与端到端交付**
- **R3. 亲自实现与系统集成**
- **R5. 评估与生产质量**
- **R6. 安全、治理、可靠性与成本**
- **R7. 采用与可量化业务影响**
- **R8. 可复用资产与现场反馈**

参见 [OpenAI 与 Amazon FDE 岗位能力框架](../../role-requirements.zh.md)。

## 引用来源

1. [Tampa General Hospital，AI 诊疗协同平台公告](https://www.tgh.org/news/tgh-press-releases/2024/june/tgh-selects-palantir-ai-software-connected-care-coordination)
2. [Tampa General Hospital，Care Coordination Center](https://www.tgh.org/about-tgh/care-coordination-center)
3. [Palantir，医院 AI 平台](https://www.palantir.com/offerings/palantir-for-hospitals/)
4. [Healthcare IT News，Tampa General 的 AI 诊疗协同实践](https://www.healthcareitnews.com/news/tampa-generals-investment-ai-enabled-care-coordination-software-saves-nearly-600-lives)
