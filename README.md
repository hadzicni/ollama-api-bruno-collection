# Ollama API - Bruno Collection

A comprehensive [Bruno](https://www.usebruno.com/) collection for the [Ollama REST API](https://docs.ollama.com/api) - local, on your network, or via Ollama Cloud.

## Contents

| Folder | Requests |
|---|---|
| Server | Health check, version, status, account, model recommendations |
| Generate | `/api/generate` - streaming, JSON/structured output, thinking, vision, fill-in-the-middle, raw mode, logprobs, load/unload |
| Chat | `/api/chat` - multi-turn, structured output, thinking, tool calling, vision, logprobs |
| Embeddings | `/api/embed`, `/api/embeddings` (legacy) |
| Models | Tags, PS, show, pull, push, copy, create, delete, blobs |
| OpenAI Compatibility | `/v1/chat/completions`, `/v1/completions`, `/v1/embeddings`, `/v1/models`, `/v1/responses` |
| Anthropic Compatibility | `/v1/messages` incl. streaming, tools, thinking, vision |
| Cloud & Web Search | Web search, web fetch, cloud models |
| Workflows | Chat history, mini RAG, model lifecycle |

## Quick Start

1. Install Bruno (YAML/OpenCollection format support required)
2. **Open Collection** and select this folder
3. Select the **Local** environment
4. Pull the models:

```bash
ollama pull llama3.2 && ollama pull qwen3 && ollama pull gemma3 && ollama pull embeddinggemma
```

For web search and cloud requests, create an API key at <https://ollama.com/settings/keys> and add it to the environment as the secret `ollamaCloudApiKey`. Secrets are not stored in the collection files.

See the collection documentation inside Bruno for more details.
