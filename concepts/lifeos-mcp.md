# LifeOS MCP Plugin Pattern

LifeOS implements a modular MCP-style plugin hub that mirrors the best community Obsidian MCP servers (Semantic Notes Vault MCP, Obsidian Intelligence, Analogy, Vault Retrieval).

## Available tools in the `obsidian` plugin
- Semantic search over the vault
- List notes
- Read note by path
- Create / update note (auto-embeds)
- Tag cloud extraction

## Design
- Vault lives at `backend/data/vault/` (plain Markdown)
- Embeddings: sentence-transformers (all-MiniLM-L6-v2) + FAISS
- Metadata + query log in SQLite
- Plugins are independent Python modules under `app/plugins/`

## Why this matters
Same pattern the community is converging on in 2026:
local embeddings + FTS/hybrid retrieval + MCP tools so any AI agent can use the vault without uploading notes.

See also: [[concepts/mcp]] · [[projects/lifeos]]
