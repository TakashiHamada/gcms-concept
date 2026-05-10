# GCMS — Concept

GCMS のシステムコンセプトをまとめた、静的な 1 枚もの HTML ページです。GitHub Pages での公開を前提にしています。

## 構成

| ファイル     | 役割                                          |
| ------------ | --------------------------------------------- |
| `index.html` | ページ本体（コンテンツとレイアウト）          |
| `styles.css` | Tailwind 上に重ねる小さなカスタムスタイル     |
| `.nojekyll`  | GitHub Pages の Jekyll 処理を無効化           |

## 使用ライブラリ（すべて CDN・ビルド不要）

- [Tailwind CSS (Play CDN)](https://tailwindcss.com/docs/installation/play-cdn) — モバイルファーストなレスポンシブ
- [highlight.js](https://highlightjs.org/) — コードブロックのシンタックスハイライト
- Google Fonts: Inter / JetBrains Mono

## ローカル確認

任意の静的サーバで `index.html` を開けば確認できます。

```bash
# 例: Python の組み込みサーバ
python3 -m http.server 8000
# → http://localhost:8000
```

## デプロイ（GitHub Pages）

1. リポジトリの **Settings → Pages**
2. Source を `Deploy from a branch` に設定
3. Branch を本ブランチ（または `main`）の `/ (root)` に設定して保存
