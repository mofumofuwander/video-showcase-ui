\# Video Showcase UI



NetflixライクなUI/UXを意識して制作した、動画・画像コンテンツのショーケースWebアプリです。  

視認性・操作感・パフォーマンスのバランスを重視し、実際のプロダクトを想定して設計しています。



---



\## 🔍 Overview



\- ヒーロースライダー + 横スクロール型の一覧レイアウト

\- Lazy Load による軽量な描画

\- 自動スライド / 一時停止 / インジケータ制御

\- Supabase を用いたデータ管理



「見て気持ちいい」「操作して迷わない」UIを目標に制作しました。



---



\## 🎯 Purpose / 背景



動画・画像を多く扱うUIでは、以下の課題が発生しがちです。



\- 初期表示が重くなる

\- スクロールや操作がカクつく

\- 現在の状態が分かりにくい



本プロジェクトでは、  

\*\*パフォーマンスとUXを両立したショーケースUI\*\* をテーマに設計しました。



---



\## 🧩 Main Features



\### Hero Slider

\- 自動スライド（一定時間で切り替え）

\- マウス操作中は一時停止

\- 進行状況を可視化するインジケータ

\- フェード + ズームによる自然なトランジション



\### Content Rows

\- カテゴリー別の横スクロールレイアウト

\- Lazy Load による描画最適化

\- アクティブ要素のみ視覚的に強調



---



\## ⚙️ Tech Stack



\- \*\*Framework\*\*: Next.js (App Router)

\- \*\*Styling\*\*: Tailwind CSS

\- \*\*Backend / DB\*\*: Supabase

\- \*\*Language\*\*: TypeScript

\- \*\*Image Optimization\*\*: next/image

\- \*\*State Management\*\*: React Hooks



---



\## 🚀 Performance Optimization



\- Heroのみ `priority` を指定し即時表示

\- 一覧画像は Lazy Load で必要時のみ読み込み

\- GPU(VRAM)管理はブラウザに委任し、不要な常駐を回避

\- 不要な再レンダリングを避ける状態設計



---



\## 🎨 UI / UX Design



\- モノトーンを基調とした落ち着いた配色

\- 情報の階層を意識したテキストコントラスト

\- 操作中の「意図しない挙動」を避ける設計

&nbsp; - マウス移動時のタイマー一時停止

&nbsp; - インジケータ進行方向の最適化



---



\## 📦 Getting Started



```bash

git clone <repository-url>

cd project

npm install

npm run dev



