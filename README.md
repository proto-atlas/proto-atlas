# proto-atlas

AI/LLMを組み込んだWebアプリケーションを開発しています。TypeScript/React/FastAPIを中心に、フロントエンドからサーバーサイドまでフルスタックで作ります。
会計・財務の学習背景があり、経理・会計領域のAI自動化にも取り組んでいます。
AIを使うときは、出力を検証し、人が確認してから確定する、という信頼性を意識した設計を大事にしています。

## 主なプロジェクト

- **keiriflow-ai**：請求書・領収書をAIで読み取り、仕訳候補の生成から警告・承認・監査ログ・CSV出力までを、人が承認してから確定する会計AIワークフロー。AI出力はZodで検証し、書き込みは承認後に限定、APIコストも制御。
- **rag-knowledge-assistant**：文書を検索して根拠付きで回答するRAGアプリ。該当文書が無いときは答えない制御、SSEでの逐次配信を実装。
- **medical-extractor**：tool_use（Function Calling）とZodの二重検証で、文書を構造化データに抽出。
- **saleslog**：React+FastAPIのフルスタックCRM。ロール別認可、AIの下書きを人が承認してから確定するワークフロー、pytest/Vitest/Playwrightとカバレッジしきい値、CI。

## 技術スタック

- **フロントエンド**：TypeScript/React/Next.js/Vue/Nuxt/Tailwind CSS
- **バックエンド・インフラ**：Python/FastAPI/SQLAlchemy、Cloudflare Workers/Durable Objects/D1/KV/Vectorize、Supabase
- **AI・LLM**：Anthropic API/OpenAI API/Workers AI、RAG、tool_use（Function Calling）、構造化出力、SSE
- **品質**：TypeScript strict/Zod/pytest/Vitest/Playwright/ruff/mypy/GitHub Actions

## 大事にしていること

- AIの出力をそのまま確定させず、検証（Zodスキーマ）と人の承認をはさむ設計にする
- 型安全とテストで、フロントエンドとサーバーサイドの両方の挙動を確かめる
- 公開デモではコストと権限を制御し、確認した範囲・していない範囲をREADMEと検証記録で追えるようにする

## リンク

- saleslog（合成データのUIデモ）：https://saleslog-demo.pages.dev/
- crypto-realtime-dashboard（デモ）：https://crypto-realtime-dashboard.pages.dev
- keiriflow-ai（閲覧は公開・操作はキー制）：https://keiriflow-ai.atlas-lab.workers.dev
