<div align="center">

# Sunish Bharathan

### I got tired of writing JQL. So I built an AI tool that does it for me.

🌐 **[atlasmind.de](https://atlasmind.de)**

*Open to interesting projects and conversations*

</div>

---

## Featured: The AtlasMind Platform

**[AtlasMind](https://atlasmind.de)** is an open-source Jira sprint visualiser built to solve a real problem Jira teams face every day: querying and visualising sprint data without writing a single line of JQL.

Ask questions in plain English, get back interactive hierarchy maps, tables, and AI-generated charts. It runs fully locally via Ollama, your Jira data never leaves your machine.

**What it took to build:**
- Local LLM orchestration with Ollama and Docker - reliable, reproducible, zero cloud cost
- Semantic search with pgvector for JQL annotation retrieval
- Self-hosted on Oracle Cloud with Caddy and Let's Encrypt
- The gap between "it works on my machine" and "it works for others" - the hardest lesson

> *AtlasMind reduced sprint query time from minutes to seconds, replacing manual JQL and EazyBi dashboard work for Jira teams.*

**[→ Try AtlasMind](https://atlasmind.de)** · **[→ Frontend UI](https://github.com/sunishbharat/AtlasMind-frontendUI)**

---

## AtlasMind-Netra: The MCP Server Layer

**[AtlasMind-Netra-mcp](https://github.com/sunishbharat/AtlasMind-Netra-mcp)** is the AI agent and MCP server that sits between any MCP-compatible client (Claude Desktop, Cursor, Claude Code) and the AtlasMind backend.

The problem it solves: Jira queries written by an LLM routinely fail because natural language is ambiguous. "Escalation" could be a label, a custom field, or a priority value. "Today" could mean created, updated, or due today. "My team" has no JQL equivalent.

Netra fixes this by running a multi-turn clarification loop before dispatching any query to Jira:
- Detects ambiguous terms and asks one targeted clarifying question using real field names from the live Jira instance
- Learns team conventions so the same question is never asked twice, persisting them across sessions
- Exposes four MCP tools publicly: `query_jira`, `generate_briefing`, `get_report`, and `get_jira_context`
- Supports both stdio (Claude Desktop) and streamable-HTTP (production, multi-user) transports

Works with Claude Desktop, Claude Code, Cursor, and any MCP-compatible client.

**[→ View the code](https://github.com/sunishbharat/AtlasMind-Netra-mcp)**

---

## Other things I've built

**[llm-from-the-ground-up](https://github.com/sunishbharat/llm-from-the-ground-up)**
I wanted to really understand transformers, so I built a GPT-2 style LLM from scratch in PyTorch. Every layer, every matrix multiply, no black boxes.

**[NaamManthan](https://github.com/sunishbharat/NaamManthan)**
A character-level generative model for Indian names, inspired by Karpathy's makemore. Small project, but one of my favourites - there's something delightful about a model that invents names.

**[docling-pgvector](https://github.com/sunishbharat/docling-pgvector)**
A RAG pipeline that turns documents into a searchable knowledge base using Docling and pgvector. The backbone of AtlasMind's JQL suggestion engine.

**[lida-ollama-extension](https://github.com/sunishbharat/lida-ollama-extension)** · **[llmx-ollama-extension](https://github.com/sunishbharat/llmx-ollama-extension)**
Extended Microsoft LIDA and llmx to support local Ollama models, because not everyone wants to send their data to the cloud.

---

## What I can help with

If you're working on something in this space, I'm happy to collaborate:

- **Jira & Atlassian tooling** - custom AI interfaces, automation, natural language querying
- **MCP servers** - building agentic tool layers for existing backends and APIs
- **Local LLM integrations** - Ollama, RAG pipelines, self-hosted AI systems
- **AI-powered dashboards** - replacing manual BI work (EazyBi, Tableau) with intelligent query layers
- **Python & FastAPI backends** - production-ready APIs with Docker and cloud deployment

---

## What I care about

I care about making AI **actually usable** - not as a demo, but as a tool that works reliably in the real world, on your own hardware, with your own data.

Local LLMs. RAG pipelines. Developer tooling. Natural language interfaces over structured systems. MCP as the connective layer between AI clients and the tools teams already use.

---

## Tech I reach for

`Python` · `FastAPI` · `FastMCP` · `Ollama` · `pgvector` · `PostgreSQL` · `Docker` · `Oracle Cloud` · `Jira REST API` · `PyTorch` · `Caddy` · `MCP` · `PydanticAI` · `Kimchi` · `LLM` · `RAG` · `Fine-tuning`

---

<div align="center">

📍 Berlin, Germany &nbsp;·&nbsp; 🌐 [atlasmind.de](https://atlasmind.de)

*Always happy to talk about local AI, Jira tooling, MCP servers, developer tools, or anything you're building.*

**[LinkedIn](https://www.linkedin.com/in/sunishbharathan)**

</div>
