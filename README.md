# GCMS — Concept

GCMS のシステムコンセプトをまとめた静的サイトです。GitHub Pages での公開を前提にしています。
現在はデザイン方向を決めるための **デザインバリアント比較フェーズ** です。

## デザインバリアント

`index.html` がピッカー（選択画面）になっており、4 種類のデザインを切り替えて比較できます。

| テーマ | パス | インスパイア元 | 特徴 |
| --- | --- | --- | --- |
| Stripe-inspired | `themes/stripe.html` | stripe.com/docs | 明るい3カラム・インディゴ・上品な情報密度 |
| Vercel-inspired | `themes/vercel.html` | vercel.com/docs | 純白とシャープな線・モノクロームミニマル |
| Linear-inspired | `themes/linear.html` | linear.app | ダーク・グラデーション・洗練された余白 |
| Anthropic-inspired | `themes/anthropic.html` | docs.anthropic.com | クリーム背景・セリフ見出し・読書体験重視 |
| Gift10-inspired    | `themes/gift10.html`    | gift10.co.jp       | 白基調 + 朱色アクセント・太めゴシック・ギャラリー風 |

各テーマページの上部に「テーマ切替バー」があり、互いに行き来できます。
気に入ったテーマが決まったら、その内容を `index.html` に昇格してください。

## ファイル構成

| ファイル                | 役割                                          |
| ----------------------- | --------------------------------------------- |
| `index.html`            | デザインピッカー                              |
| `themes/*.html`         | 各テーマのバリアント                          |
| `styles.css`            | 共通の小さなカスタムスタイル                  |
| `.nojekyll`             | GitHub Pages の Jekyll 処理を無効化           |

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
