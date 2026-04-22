# ai-video-factory

アニメスタイル商品紹介動画の自動生成パイプライン。

毎週トレンド調査 → 毎日Vidu Q3で自動生成。

## 構成

| ファイル | 内容 |
|---------|------|
| `themes.md` | 週次テーマ・プロンプト（毎週日曜AM1時更新） |
| `logs/YYYY-MM-DD.md` | 日次生成ログ（task_id・プロンプト・意図） |

## 動画ダウンロード

```bash
vidu-cli task get <task_id> --output ./downloads
```

## スケジュール

- 調査：毎週日曜 AM1:00 JST
- 生成：毎日 AM4:00 JST
