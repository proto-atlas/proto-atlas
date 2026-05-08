# proto-atlas

TypeScript / React / Next.js / Nuxt / Cloudflare Workers を使い、AI / LLM を組み込んだWebアプリを制作しています。
直近では、リアルタイムUI、Human-in-the-loop型の業務ワークフロー、RAG、引用付きQ&A、構造化抽出を題材にした公開デモを整備しています。

## 主な技術

TypeScript / JavaScript / React / Next.js / Vue / Nuxt / Tailwind CSS
Cloudflare Workers / Durable Objects / KV / D1 / Vectorize / Supabase
Playwright / Vitest / GitHub Actions
Anthropic API / OpenAI API / RAG / SSE

## 主な公開プロジェクト

### Crypto Real-time Dashboard

暗号資産の公開マーケットデータを題材にした、リアルタイム更新ダッシュボードです。
Demo Mode、Live REST、Live WebSocket、WebSocket fallback、10万件の仮想取引履歴テーブル、仮想ポートフォリオ、dark/light theme、Playwright E2Eを実装しています。

- Demo: https://crypto-realtime-dashboard.pages.dev
- GitHub: https://github.com/proto-atlas/crypto-realtime-dashboard

### KeiriFlow AI

請求書・領収書をAIで読み取り、仕訳候補、警告、承認、監査ログ、CSV出力までを扱う Human-in-the-loop 型の会計AIワークフローデモです。
公開URLでは合成データの読み取り画面を確認でき、変更系API、AI候補生成、CSV出力は確認用access keyでguardしています。

- Demo: https://keiriflow-ai.atlas-lab.workers.dev
- GitHub: https://github.com/proto-atlas/keiriflow-ai

### RAG Knowledge Assistant

架空文書コーパスを使ったRAGデモです。
未認証トップページとaccess key付き限定live RAG経路を分け、Workers AI / Vectorize / D1 / Anthropic、no-answer制御、source id validation、SSE streaming、cost guardを実装しています。

- Demo: https://rag-knowledge-assistant.atlas-lab.workers.dev
- GitHub: https://github.com/proto-atlas/rag-knowledge-assistant

## 関連プロジェクト

### Citation Reader

PDFまたはテキストを対象にした、引用元付きAI要約・Q&Aアプリです。
Anthropic Citations API、Prompt Caching、SSE streaming、citation validation、5ブラウザE2Eを実装しています。

- Demo: https://citation-reader.atlas-lab.workers.dev
- GitHub: https://github.com/proto-atlas/citation-reader

### Medical Extractor

架空の医療文書をSOAP形式へ構造化抽出するデモです。
Anthropic tool_use、Zod strict schema、source_text検証、PHIや診断用途ではないことの明示を実装しています。

- Demo: https://medical-extractor.atlas-lab.workers.dev
- GitHub: https://github.com/proto-atlas/medical-extractor

### Nuxt AI Blog

Nuxt 4 / Vue / TypeScriptで作成した技術ブログです。
記事一覧、検索、タグ、記事詳細、AI要約、Cloudflare Workers公開、Durable Objectsによるsummary cache / quota設計を実装しています。

- Demo: https://nuxt-ai-blog.atlas-lab.workers.dev
- GitHub: https://github.com/proto-atlas/nuxt-ai-blog

## 補足

一部のlive AI / live RAG / 変更系APIは、コスト管理と乱用防止のため確認用access keyで保護しています。
公開URLでは、キーなしで確認できる範囲、スクリーンショット、README、設計資料、検証証跡を確認できます。live操作が必要な場合は個別に共有します。

## Interests

フロントエンド開発、AI / LLMを活用したWebアプリ開発、RAG、引用付き回答、構造化出力、Cloudflare Workersを使った軽量な本番公開に関心があります。
