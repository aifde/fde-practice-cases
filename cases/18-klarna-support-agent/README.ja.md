# 18. Klarna：返金と返品につながる多言語サポート

~~~mermaid
flowchart LR
  A[顧客対話と注文状態] --> B[多言語AIアシスタント]
  B --> C[返金、返品、引継ぎ]
  C --> D[顧客の解決]
~~~

**導入。** KlarnaはAIアシスタントを、注文情報、返金、返品を伴うサポート業務につなぎ、静的なFAQに留めませんでした。

**FDEの示唆。** 検証可能なバックエンド操作へ接続し、例外は人へ渡します。OpenAIは初月230万件の対話、再問い合わせ25% 減、完了時間が11分から2分未満へ短縮したと公表しています。

## 参考資料

1. [出典：OpenAI、Klarna](https://openai.com/index/klarna/)

[中文](README.md) | [English](README.en.md) | 日本語
