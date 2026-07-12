# 23. Decagon：把客服代理接到企业数据和业务规则

[来源：Anthropic Decagon 案例](https://www.anthropic.com/customers/decagon)

~~~mermaid
flowchart LR
  A[工单和客户数据库] --> B[政策感知代理]
  B --> C[查询资格并执行任务]
  C --> D[例外转人工]
~~~

**问题与交付。** 企业客服常被泛化聊天机器人拖累：能回答却不能完成退款、资格验证或复杂流程。Decagon 把代理连接到现有工单与客户系统，并让其遵循品牌和业务规则。

**公开成果与 FDE 启示。** 案例称过度推断率下降 70%。可复用方法是把代理能做的动作、所需证据、拒绝条件和人工接管路径写成可测试的策略，而不是单靠系统提示。

中文 | [English](README.en.md) | [日本語](README.ja.md)
