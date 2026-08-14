# proto-atlas

Web制作の受託とフリーランスを経て、TypeScriptとReactを中心にWebアプリを個人開発しています。
フロントエンドの実装に加えて、Cloudflare Workersでのサーバーサイド実装や、LLMを組み込んだアプリも作っています。

## 主なプロジェクト

- **[crypto-realtime-dashboard](https://github.com/proto-atlas/crypto-realtime-dashboard)**
  暗号資産の公開マーケットデータをリアルタイムに可視化するWebアプリ。10万件の仮想スクロールテーブル、BFF Worker経由でのデータ取得、配信元が落ちたときの自動切り替えを実装しました。[デモ](https://crypto-realtime-dashboard.pages.dev)

- **[offline-llm-eval](https://github.com/proto-atlas/offline-llm-eval)**
  RAGやLLMの回答を、外部APIに依存せず評価するPython製のワークベンチ。引用の整合性や応答形式を検査します。

- **[keiriflow-ai](https://github.com/proto-atlas/keiriflow-ai)**
  請求書をAIで読み取り、読取結果を人が確認・承認してから確定する仕組み。AIの出力はZodで検証しています。

- **[rag-knowledge-assistant](https://github.com/proto-atlas/rag-knowledge-assistant)**
  文書を検索して根拠付きで回答するRAGアプリ。該当する文書がないときは回答を生成しない制御と、SSEで回答を少しずつ送る処理を実装しました。

## 使っている技術

- **フロントエンド** TypeScript, React, Next.js, Vue, Nuxt, Tailwind CSS
- **サーバーサイド・基盤** Cloudflare Workers, Durable Objects, D1, KV, Vectorize, Hono, Python, FastAPI, Supabase
- **AI・LLM** Anthropic API（tool_use, Citations, Prompt Caching）, RAG, SSE
- **テスト・品質** TypeScript strict, Zod, Vitest, Playwright, pytest, GitHub Actions

## 開発で決めていること

- 外部APIやAIの出力はそのまま画面に出さず、スキーマで検証してから扱う
- 公開しているデモは、外部APIを使わない状態を初期表示にして、実際の接続は操作したときだけ有効にする
- 確認した範囲と確認していない範囲を、READMEと検証記録に書き残す
