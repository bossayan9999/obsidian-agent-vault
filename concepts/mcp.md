# Model Context Protocol (MCP) in this project

This app implements an MCP-*style* tool registry:

- Tools are registered with name, description, and input schema
- The agent (LLM) decides which tools to call
- Tools execute and return structured results
- Results are injected into the final answer generation context

Available tools:
- `web_search`
- `calculator`
- `code_execute` (sandboxed expressions only)
- `get_datetime`
- Memory search against this vault
