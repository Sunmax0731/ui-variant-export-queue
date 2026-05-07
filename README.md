# UIバリアント書き出しキュー

ui-variant-export-queue は UI素材を複数解像度/状態で書き出す制作者 向けの closed alpha プロダクトです。UIパーツ、状態、解像度、出力先、キュー状態を定義して書き出し前に検査する。

## Source

- PICKUP Rank: 55
- Domain / Idea No: AssetPipeline / 6
- Repository: ui-variant-export-queue
- 主な公開先: GitHub Release / BOOTH
- created_idea: `D:/AI/AssetPipeline/created_idea_006_ui-variant-export-queue`
- 同梱ZIP: `D:/AI/AssetPipeline/created_idea_006_ui-variant-export-queue/idea_006_ui-variant-export-queue.zip`
- 開始時 README: 存在しない


## Alpha Scope

- 代表シナリオ4件の自動検証
- 必須項目不足、警告、混在バッチの分類
- src/cli/ のホスト連携シェル
- QCDS、security/privacy、traceability、release checklist、manual test docs
- docs ZIP: `dist/ui-variant-export-queue-docs.zip`

## Commands

```powershell
npm test
node src/cli/index.js samples/representative-suite.json
npm run build:docs
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` にあります。

