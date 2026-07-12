# 06. 加拿大阿尔伯塔省政府：AI 辅助遗留系统安全修复

~~~mermaid
flowchart LR
  A[政府应用代码库] --> B[自动化检查代理]
  B --> C[安全团队验证修复]
  C --> D[上线与白皮书复用]
~~~

**问题与交付。** 政府遗留系统规模大、文档不全，安全审查很难覆盖。省技术团队用 Claude Code 做批量检查和修复，再由安全与工程人员验证，避免把模型输出直接当作生产变更。

**公开成果与 FDE 启示。** 公开案例称团队在 20 小时内扫描 4.66 亿行代码。可复用方法是将代理定位为高覆盖率的发现与初修工具，以人工验收、变更控制和可公开复盘来守住风险边界。

## 二、工业、能源与供应链

## 引用来源

1. [来源：Anthropic 阿尔伯塔政府案例](https://www.anthropic.com/news/alberta-government-claude-cybersecurity)

中文 | [English](README.en.md) | [日本語](README.ja.md)
