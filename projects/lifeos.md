# LifeOS

**Local-first AI Knowledge Base with MCP Plugin Hub**

Repo: https://github.com/bossayan9999/lifeos

## Summary
Full-stack system that turns an Obsidian-style Markdown vault into a queryable knowledge base with:
- Semantic search (FAISS + sentence-transformers)
- MCP Plugin Hub (obsidian, crm, code_repo, analytics…)
- React chat UI with citations and confidence scores
- Data Cleaner + feedback / knowledge-gap loop

## Key design principles
- Local-first retrieval
- External calls (web / LLM) only when local confidence is low
- All internal data stays private
- Plugins are modular and replaceable

## Related notes
- [[concepts/mcp]]
- [[concepts/agentic-loops]]
- [[projects/fast-agentic-ai]]

## Status
Core scaffold + working plugins implemented (2026-08-02).
