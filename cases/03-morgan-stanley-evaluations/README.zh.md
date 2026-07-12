# 03. Morgan Stanley：评估先行的受监管财富管理 AI

[English](README.md) | 中文 | [日本語](README.ja.md)

| 项目 | 证据 |
| --- | --- |
| 置信度 | 高 |
| 部署状态 | 已进入生产，并在财富管理团队全面推广 |
| 客户 | Morgan Stanley Wealth Management |
| 交付方 | OpenAI |
| AI 场景 | 内部知识检索、研究摘要、会议纪要、后续邮件草稿和 CRM 写回 |
| 与 AI FDE 的关系 | 客户团队与模型团队先建立代表性评估、检索方法和合规控制，再扩大使用范围 |

## 业务问题

财富顾问需要快速访问大量经过批准的研究和内部知识。在受监管环境中，一个听起来合理但没有依据的回答不可接受。会议摘要还有额外要求：系统必须准确提取行动项、取得客户同意，并让顾问对最终记录和沟通负责。

Morgan Stanley 与 OpenAI 因此把评估当成产品本身，而不是上线前的最后一项测试。首批目标很窄：提高信息检索速度、总结获批材料，并在不移除专业判断的前提下帮助顾问准备工作。

## 交付过程

在 AI @ Morgan Stanley Assistant 项目中，团队使用真实顾问问题测试模型，由顾问和提示词工程师评价准确性和连贯性。随着文档库扩大，双方继续调整检索方法和评估集。公开案例称，系统从只能覆盖约 7,000 个问题，发展到可在 10 万份文档中处理顾问查询。

后续产品 AI @ Morgan Stanley Debrief 会把获得客户同意的会议录音转成纪要、行动项和后续邮件草稿。顾问必须在发送或归档前复核，之后才能把纪要写入 Salesforce。

~~~mermaid
flowchart LR
  A[获批研究与内部文档] --> B[检索系统]
  B --> C[助手回答]
  D[经客户同意的会议录音] --> E[转写与摘要]
  E --> F[纪要、行动项和邮件草稿]
  C --> G[顾问复核]
  F --> G
  G --> H[客户沟通或 CRM 记录]
  H --> I[专家反馈与回归用例]
  I --> B
  I --> E
~~~

## 评估与治理

- 顾问和提示词工程师用真实问题评价回答。
- 摘要评估检查关键信息是否保留，以及是否引入错误。
- 团队为多语言客户加入翻译评估。
- Debrief 使用不同会议类型构建数据集，测试行动项提取。
- 每日回归测试检查质量和合规弱点。
- 顾问保留纪要与沟通内容的最终批准权。
- Morgan Stanley 把零数据保留视为合作中的重要安全条件。

企业评估不只是一个准确率，它还包括代表性数据、专业判断、回归测试、检索质量、客户同意和工作流权限。

## 公开结果

OpenAI 与 Morgan Stanley 披露：

- 财富顾问团队采用率超过 98%。
- 可访问文档比例从约 20% 提高到 80%。
- 产品从 Assistant 扩展到 Debrief，并继续规划其他场景。
- 部分原本需要数天的跟进工作缩短到数小时。

Morgan Stanley 在 2024 年 6 月发布 Debrief 时，也确认了 98% 的采用率。

## 为什么属于高置信度 AI FDE 案例

项目把需求发现、受监管知识、检索工程、评估、安全、客户同意、人工复核和 CRM 集成连接在一起。评估资产还被复用于多个产品，现场反馈会继续影响检索方法和后续产品方向。

## 尚未证明的部分

- 评估数据集、评分者、阈值和错误率没有公开。
- 高采用率不能单独证明投资回报或客户结果改善。
- 大部分性能数字来自参与机构。
- AI 的影响无法与培训、流程重构和平台改进完全分离。

## FDE 岗位能力对应

- **R1. 嵌入式需求发现与可信协作**
- **R3. 亲自实现与系统集成**
- **R4. AI 工作流与人工控制设计**
- **R5. 评估与生产质量**
- **R6. 安全、治理、可靠性与成本**
- **R7. 采用与可量化业务影响**
- **R8. 可复用资产与现场反馈**

参见 [OpenAI 与 Amazon FDE 岗位能力框架](../../role-requirements.zh.md)。

## 引用来源

1. [OpenAI，Morgan Stanley 评估体系案例](https://openai.com/index/morgan-stanley/)
2. [Morgan Stanley，AI @ Morgan Stanley Debrief 发布公告](https://www.morganstanley.com/press-releases/ai-at-morgan-stanley-debrief-launch)
3. [Morgan Stanley，Insights and Outcomes, Volume 6](https://www.morganstanley.com/cs/pdf/FOR-Insights-and-Outcomes-VOL6-layout-ebook-digital.pdf)
