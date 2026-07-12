# 29. Notion：ワークスペース検索の精密な再順位付け

[出典：Cohere、Notion](https://cohere.com/fr/customer-stories/notion)

~~~mermaid
flowchart LR
  A[Notion、Slack、Driveの内容] --> B[候補検索]
  B --> C[再順位付けと回答生成]
  C --> D[多言語チーム]
~~~

**導入。** Notionはワークスペースと接続ツールをまたぐ検索パイプラインへ再順位付けを入れ、変動する需要にはクラウドの拡張性で対応しました。

**FDEの示唆。** ワークスペース規模に応じて検索経路を分け、実際に失敗した検索で再現率と順位付けを改善します。事例は精度、コスト、多言語体験を同時の目標として扱います。

[中文](README.md) | [English](README.en.md) | 日本語
