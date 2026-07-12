# 09. Heineken USA：販売網の欠品予防

~~~mermaid
flowchart LR
  A[醸造所、倉庫、販売店データ] --> B[ライブ供給網表示]
  B --> C[欠品リスクと配送変更]
  C --> D[供給網の実行]
~~~

**導入。** 生産、倉庫、顧客、船舶のデータを接続し、混乱を早く把握して配送計画を調整します。

**FDEの示唆。** 再現可能な例外キューで始めます。公開資料では、2日間の試験で約30万ドル相当の25件の販売店アラートを解決したとされます。

## 参考資料

1. [出典：Palantir Impact](https://www.palantir.com/impact/)

[中文](README.md) | [English](README.en.md) | 日本語
