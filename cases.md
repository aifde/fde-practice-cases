# 30 个 AI FDE 式落地案例

中文 | [English](README.en.md) | [日本語](README.ja.md)

## 案例选择口径

FDE 的价值不在于单独展示模型，而在于把领域问题、数据/系统、用户工作流、风险控制和可量化结果接成一个可迭代的交付回路。本页把有现场交付特征的公开案例归为 FDE 式案例：有的来自明确的现场/实施团队，有的是客户与供应商共同完成的嵌入式交付。

每个条目均链接到公开一手资料。来源中的成果与数字均为发布方披露；没有公开量化结果时，本文不补造数字。

## 分类索引

### 一、高风险公共服务与临床运营

1. [美国陆军 TITAN：边缘传感器到目标情报](cases/01-us-army-titan/)
2. [NHS Federated Data Platform：把患者流转做成可执行工作流](cases/02-nhs-federated-data-platform/)
3. [Tampa General Hospital：飓风压力下的患者与人力调度](cases/03-tampa-general-hospital/)
4. [Cleveland Clinic：虚拟指挥中心优化医院资源](cases/04-cleveland-clinic-command-center/)
5. [HCA Healthcare：把排班质量变成可解释的运营信号](cases/05-hca-healthcare-scheduling/)
6. [加拿大阿尔伯塔省政府：AI 辅助遗留系统安全修复](cases/06-alberta-government-cybersecurity/)

### 二、工业、能源与供应链

7. [Panasonic Energy：电池工厂的维护知识副驾](cases/07-panasonic-energy-maintenance/)
8. [Komatsu：矿山设备服务与停机时间](cases/08-komatsu-equipment-uptime/)
9. [Heineken USA：经销链路中的缺货预警](cases/09-heineken-stockout-prevention/)
10. [Wendy’s QSCC：餐饮供应与资源重平衡](cases/10-wendys-inventory-balancing/)
11. [Eaton：供应链数字化优先级](cases/11-eaton-supply-chain/)
12. [Doosan Infracore：重型机械的产品与现场反馈](cases/12-doosan-field-feedback/)
13. [Sarcos：机器人与边缘 AI 的现场协同](cases/13-sarcos-edge-ai/)
14. [Focus Brands：从第一批应用到可复制运营平台](cases/14-focus-brands-platform/)

### 三、金融、生命科学与知识工作

15. [Morgan Stanley：受监管财富管理中的评估先行](cases/15-morgan-stanley-evaluations/)
16. [BBVA：从受控试点到全行 AI 采用](cases/16-bbva-ai-adoption/)
17. [Moderna：把研发判断保留在人类临床团队手中](cases/17-moderna-clinical-ai/)
18. [Klarna：把多语言客服代理接进退款与退货流程](cases/18-klarna-support-agent/)
19. [GitLab：用企业 AI 改造内部协作而非只做产品功能](cases/19-gitlab-enterprise-ai/)
20. [Quantium：咨询团队的“每人每天 AI”](cases/20-quantium-ai-adoption/)
21. [Headstart：AI 原生软件项目的交付节奏](cases/21-headstart-ai-native-delivery/)
22. [Section：把 AI 采用做成能力建设产品](cases/22-section-ai-capability/)

### 四、客服、企业搜索与工作流代理

23. [Decagon：把客服代理接到企业数据和业务规则](cases/23-decagon-policy-agent/)
24. [Assembled：客服代理与人工队列协同](cases/24-assembled-human-ai-support/)
25. [Lyft：以品牌语气与准确性选择客服模型](cases/25-lyft-support-model/)
26. [Smartsheet：三种表面上的企业级 AI 部署](cases/26-smartsheet-ai-surfaces/)
27. [CoreWeave：90 天内把代理嵌入 Slack 支持链路](cases/27-coreweave-slack-agent/)
28. [Draftwise：合同起草中的可追溯检索](cases/28-draftwise-legal-rag/)
29. [Notion：工作区搜索的精准重排](cases/29-notion-rerank-search/)
30. [Oracle Fusion：把 100 多个生成式用例嵌入业务套件](cases/30-oracle-fusion-ai/)

## 跨案例可复用的方法

1. **从决策点而非模型开始。** 先明确谁在什么时刻做什么决定，TITAN、医院指挥中心和供应链例外管理都遵循这一顺序。
2. **把数据、权限和写回设计在第一天。** 能读取但不能解释、不能行动、不能追责的助手很难留在生产环境。
3. **用领域专家建立评估集。** Morgan Stanley、Draftwise 和客服案例都把真实问题与人工评分当作迭代燃料。
4. **把人工接管视为产品功能。** 临床、金融与客服系统都需要清晰的拒绝、升级和最终确认点。
5. **以工作流指标衡量。** 关注解决时长、等待天数、缺货、首次修复率、CSAT、返工率和采用率，而不只看聊天次数。
6. **首个用例要留下可复用底座。** Focus Brands、Oracle 和 NHS FDP 说明，数据对象、治理、培训和发布机制才能让第二十个用例更快。

## 研究来源说明

本页于 2026 年 7 月整理。所有链接均指向公开资料的原始发布方；页面会随时间更新，建议在采用具体数字或架构前再次核验原文与适用的本地法规。
