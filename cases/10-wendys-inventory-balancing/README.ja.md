# 10. Wendy's QSCC：レストラン網の在庫バランス

~~~mermaid
flowchart LR
  A[注文、在庫、配送センターデータ] --> B[レストラン供給モデル]
  B --> C[不足と再配分の選択]
  C --> D[運用承認]
~~~

**導入。** Wendy's QSCCは広いレストラン網の注文と在庫を追跡し、配送センターの必要量をモデル化して資源再配分を支援します。

**FDEの示唆。** 決定権をシステムに組み込みます。不足予測には責任者、エスカレーション経路、運用上のトレードオフ説明が必要です。

## 参考資料

1. [出典：Palantir Impact](https://www.palantir.com/impact/)

[中文](README.md) | [English](README.en.md) | 日本語
