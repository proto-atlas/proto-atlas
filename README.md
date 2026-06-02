# proto-atlas

TypeScript / React / Cloudflare Workers を中心に、AI / LLM を組み込んだWebアプリケーションや、開発中の挙動を後から確認するための小さなツールを作っています。

画面実装では、検索、一覧、フォーム、ストリーミング表示、根拠表示、エラー時の表示など、利用者が操作する部分の分かりやすさを重視しています。AI / LLMを使う機能では、回答結果をその場限りにせず、引用、判定条件、検証記録、再実行できるテストと合わせて確認できる形にしています。

## 主な技術

TypeScript / JavaScript / React / Next.js / Vue / Nuxt / Tailwind CSS  
Cloudflare Workers / Durable Objects / KV / D1 / Vectorize / Supabase  
Python / FastAPI / SQLAlchemy / Pydantic / SQLite  
Playwright / Vitest / node:test / pytest / ruff / mypy / GitHub Actions  
Anthropic API / OpenAI API / Workers AI / RAG / SSE

## 作っているもの

- React / TypeScript を使ったWebアプリケーション
- Cloudflare Workers を使ったAPIと公開デモ
- RAG、引用付き回答、構造化出力を扱うAI / LLM機能
- SSEストリームやLLM回答を後から確認するためのローカルツール
- テスト、検証記録、README、docsを含めた再確認しやすい開発資料

## 補足

一部のlive AI / live RAG / 変更系APIは、コスト管理と乱用防止のため確認用access keyで保護しています。公開URLでは、キーなしで確認できる範囲、スクリーンショット、README、設計資料、検証記録を確認できます。

## Interests

フロントエンド開発、AI / LLMを活用したWebアプリ開発、RAG、引用付き回答、構造化出力、Cloudflare Workersを使った軽量な公開環境に関心があります。
