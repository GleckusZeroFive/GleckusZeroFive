# Hi, I'm Vladislav Pestov

**AI/ML Engineer** from Krasnoyarsk, Russia

I build AI-powered products end-to-end: from model selection and prompt engineering to production deployment with Docker.

## What I Do

- **RAG Systems** — LangChain, hybrid search (BM25 + semantic + RRF), vector databases (Qdrant, pgvector), Russian-language lemmatization
- **LLM Integration** — Claude API, OpenAI API, local inference (Ollama, RTX 5060), prompt engineering, agent architectures
- **LangGraph Pipelines** — StateGraph with quality loops, fact-checking, judge models, revise flows
- **Telegram Bots** — aiogram 3, async Python, complex dialogue flows, voice messages (Whisper STT)
- **Workflow Automation** — n8n, Orchestrator + Worker pattern, structured JSON contracts
- **MCP Servers** — custom Model Context Protocol servers for AI agents (FastMCP, Node.js)
- **Backend** — FastAPI, PostgreSQL, Docker, Linux

## Commercial Projects

Projects delivered for clients via freelance platforms.

**AI Consultant Chatbot for a Building Materials Store**
Self-hosted LLM platform with a product knowledge base, automated cost calculations, and a custom JS widget with SSE streaming deployed on the client's website.

**Stack:** Dify (self-hosted), Google Gemini, Docker, Nginx, JavaScript

**Gamification & AI Coach for a Health-Tech Telegram Bot**
Streak/milestone system with comeback detection, AI-powered personalized nutrition and fitness coaching with trial/paywall flow. Integrated into an existing production codebase via 17+ pull requests, code review, working with the client's team.

**Stack:** Python, aiogram 3, PostgreSQL, Redis, Docker, Alembic, APScheduler

## Featured Projects

### [sciwriter-mas](https://github.com/GleckusZeroFive/sciwriter-mas)
Content generation factory with a LangGraph quality pipeline: `fetch_sources → research → write → fact_check → rate → revise loop`. Judge model (Cerebras Qwen 235B MoE) scores each draft 0–100, revises until it clears a 90 threshold. Pipeline registry lets you plug in a new writer model in one entry. Content Factory: 4 collectors (HN, arXiv, TechCrunch, Reddit) → topic ranker → generation → PostgreSQL.

**Stack:** LangGraph, Groq, Cerebras, OpenRouter, PostgreSQL, Qdrant, DuckDuckGo, Streamlit, Docker

### [telegram-bot-templates](https://github.com/GleckusZeroFive/telegram-bot-templates)
RAG platform for Telegram — one Docker image, 5 products via YAML presets (HR, Support, Legal, Tutor, Voice). Hybrid search (BM25 + semantic + RRF), ONNX intent classifier (3.7ms), voice messages (Whisper STT), streaming answers.

**Stack:** Python, aiogram 3, Qdrant, Ollama (Qwen3 8B), ONNX Runtime, Docker

### [intent-classifier](https://github.com/GleckusZeroFive/intent-classifier)
Fine-tuned ruBERT-tiny2 (29M params) for intent classification: rag/chat/followup. **F1 = 0.90**, 3.7 ms inference on CPU, ~117 MB ONNX. Published on [HuggingFace](https://huggingface.co/Gleckus/intent-classifier-rubert-tiny2) under MIT license. Full cycle documentation: PROBLEM → SOLUTION → REVIEW → REPRODUCE → ANALYSIS.

**Stack:** HuggingFace Transformers, ONNX Runtime, Google Colab

### [jobius-bot](https://github.com/GleckusZeroFive/jobius-bot)
AI job search assistant for Telegram. Scrapes hh.ru, understands user intent via regex + LLM fallback, cache of 15 779 cities, favorites system, AI career consultant. Fully async.

**Stack:** Python 3.12, aiogram 3.15, Ollama (Qwen3 8B), aiosqlite, aiohttp, pydantic

### [n8n-orchestrator-worker](https://github.com/GleckusZeroFive/n8n-orchestrator-worker)
Modular n8n automation system with Orchestrator + Worker architecture, NL intent detection, PostgreSQL session state (Supabase), and 3-level error handling with execution journal. Structured JSON contracts between steps.

**Stack:** n8n, PostgreSQL, Supabase, Webhook API, JSON contracts

## MCP Servers (custom tooling)

Own Model Context Protocol servers for AI agents — a rare stack that most developers haven't touched yet.

- **Telegram MCP** — 11 tools for Telegram (send, read, search, forward, files). Lazy connect, auto-disconnect after 120 s. FastMCP + Telethon.
- **Canvas MCP** — 22 tools for an Electron canvas (shapes, text, layers, grid). Lazy Electron start, auto-shutdown after 60 s.
- **Audio/Video MCP** — transcription (faster-whisper), 527-class sound detection, emotions, speaker diarization, video analysis. GPU inference on RTX 5060.

## Tech Stack

```
Python       | FastAPI      | aiogram 3    | asyncio
PostgreSQL   | pgvector     | Qdrant       | Redis
Docker       | Linux        | Git          | n8n
LangChain    | LangGraph    | RAG          | HuggingFace
Claude API   | OpenAI API   | Ollama       | Fine-tuning
ONNX Runtime | Whisper STT  | NLP          | Prompt Engineering
MCP          | FastMCP      | Pydantic     | SQLAlchemy
```

**Hardware:** RTX 5060, 64 GB RAM — local inference when API pricing or privacy rules out hosted models.

## Contact

- **HH.ru:** [resume (ML Engineer)](https://hh.ru/resume/9bc1ce37ff0fe443f90039ed1f4f66326c4e34)
- **Kwork:** [gleckus19](https://kwork.ru/user/gleckus19)
- **Telegram:** [@gleckus](https://t.me/gleckus)
- **Email:** lpflash@mail.ru
- **Location:** Krasnoyarsk, Russia
