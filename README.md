# 🦙 Ollama API – Bruno Collection

Eine umfangreiche [Bruno](https://www.usebruno.com/)-Collection für die [Ollama REST API](https://docs.ollama.com/api) – lokal, im Netzwerk oder über Ollama Cloud.

## Inhalt

| Ordner | Requests |
|---|---|
| 🖥️ Server | Health Check, Version, Status, Account, Modell-Empfehlungen |
| ✍️ Generate | `/api/generate` – Streaming, JSON/Structured Output, Thinking, Vision, Fill-in-the-Middle, Raw, Logprobs, Load/Unload |
| 💬 Chat | `/api/chat` – Multi-Turn, Structured Output, Thinking, Tool Calling, Vision, Logprobs |
| 🧮 Embeddings | `/api/embed`, `/api/embeddings` (Legacy) |
| 📦 Models | Tags, PS, Show, Pull, Push, Copy, Create, Delete, Blobs |
| 🔌 OpenAI Compatibility | `/v1/chat/completions`, `/v1/completions`, `/v1/embeddings`, `/v1/models`, `/v1/responses` |
| 🅰️ Anthropic Compatibility | `/v1/messages` inkl. Streaming, Tools, Thinking, Vision |
| ☁️ Cloud & Web Search | Web Search, Web Fetch, Cloud-Modelle |
| 🔁 Workflows | Chat-Verlauf, Mini-RAG, Modell-Lebenszyklus |

## Schnellstart

1. Bruno (≥ 3.0, YAML/OpenCollection-Format) installieren
2. **Open Collection** → diesen Ordner wählen
3. Umgebung **Local** auswählen
4. Modelle laden:

```bash
ollama pull llama3.2 && ollama pull qwen3 && ollama pull gemma3 && ollama pull embeddinggemma
```

Für Web Search & Cloud einen API-Key unter <https://ollama.com/settings/keys> erstellen und in der Umgebung als Secret `ollamaCloudApiKey` eintragen. Secrets werden nicht in den Dateien gespeichert.

Weitere Details stehen in der Collection-Dokumentation in Bruno.
