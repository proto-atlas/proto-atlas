# proto-atlas

Web制作経験を土台に、TypeScript / React / Nuxt / Cloudflare Workers を使ったWebアプリ開発へ領域を広げています。  
直近では、AI要約、構造化抽出、引用付きQ&A、RAG demo など、LLMを活用したWebアプリを公開しています。

## 主な技術

TypeScript / JavaScript / React / Next.js / Vue / Nuxt / Tailwind CSS  
Cloudflare Workers / Durable Objects / D1 / Vectorize  
Playwright / Vitest / GitHub Actions  
Anthropic API / OpenAI API / RAG / SSE

## Portfolio

### RAG Knowledge Assistant
Workers AI / Vectorize / D1 / Anthropic を組み合わせたRAGデモです。  
未認証トップページと access key付き限定live RAG demo を分け、no-answer、source id validation、SSE streaming、cost guard を実装しています。

- Demo: https://rag-knowledge-assistant.atlas-lab.workers.dev
- GitHub: https://github.com/proto-atlas/rag-knowledge-assistant

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

## Notes

AI APIを利用する機能は、課金・乱用防止のため一部 access key で保護しています。  
公開URLでは、概要、UI、スクリーンショット、README、検証証跡を確認できます。面接時には必要に応じて限定live demoを共有します。

## Interests

フロントエンド開発、AI / LLMを活用したWebアプリ開発、RAG、引用付き回答、構造化出力、Cloudflare Workersを使った軽量な本番公開に関心があります。
