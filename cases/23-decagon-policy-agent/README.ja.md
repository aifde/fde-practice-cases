# 23. Decagon：データと業務規則につながるサポートエージェント

[出典：Anthropic、Decagon](https://www.anthropic.com/customers/decagon)

~~~mermaid
flowchart LR
  A[チケットと顧客記録] --> B[規則を理解するエージェント]
  B --> C[適格性確認とタスク実行]
  C --> D[例外の人手引継ぎ]
~~~

**導入。** DecagonはAIエージェントを既存のチケットと顧客システムに接続し、方針に従って業務を完了できるようにしています。

**FDEの示唆。** 許可された操作、必要な根拠、拒否条件、人への引継ぎをテスト可能な方針として定義します。事例では過剰推論が70% 減ったとされています。

[中文](README.md) | [English](README.en.md) | 日本語
