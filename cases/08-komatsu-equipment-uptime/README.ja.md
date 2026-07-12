# 08. Komatsu：鉱山機械の稼働率を支えるサービス優先度

~~~mermaid
flowchart LR
  A[遠隔計測と整備履歴] --> B[資産健全性モデル]
  B --> C[サービス優先度]
  C --> D[現場サービスチーム]
~~~

**導入。** KomatsuはFoundryとAIPを使い、機器情報とサービス情報を結び、運用の改善と稼働率向上を目指しています。

**FDEの示唆。** 一般的な予知保全から始めません。まず、いつサービスチームが介入するかという一つの現場判断を選び、停止時間、初回修理率、利用率を測ります。

## 参考資料

1. [出典：Palantir Master Classes](https://www.palantir.com/master-classes/)

[中文](README.md) | [English](README.en.md) | 日本語
