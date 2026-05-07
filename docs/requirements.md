# 要件定義

## 目的

UIバリアント書き出しキュー は、UI素材を複数解像度/状態で書き出す制作者 が UIパーツ、状態、解像度、出力先、キュー状態を定義して書き出し前に検査する。

## Source

- PICKUP Rank: 55
- Domain / Idea No: AssetPipeline / 6
- Repository: ui-variant-export-queue
- created_idea: `D:/AI/AssetPipeline/created_idea_006_ui-variant-export-queue`
- ZIP: `D:/AI/AssetPipeline/created_idea_006_ui-variant-export-queue/idea_006_ui-variant-export-queue.zip`
- README確認: 開始時点では正式 repo が存在しないため、README.md は存在しない。

## Functional Requirements

- R1: componentName、variant、density、outputPath を必須項目として検査する。
- R2: 必須項目不足は fail として分類する。
- R3: `missingRetina` が true の場合は warning として分類し、手動確認理由を返す。
- R4: 複数アイテムの mixed-batch を pass / warning / fail に集計する。
- R5: 結果を CLI と docs/release evidence で再利用できる形にする。

## Non Functional Requirements

- UTF-8 で Markdown / JSON / JS / HTML / Python を保存する。
- 外部通信を既定で行わず、サンプルとローカル入力だけで検証できる。
- 手動テスト未実施であることを release 前 docs に明記する。

