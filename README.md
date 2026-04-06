# Hi, I'm Vladislav Pestov

**AI/ML Engineer** from Krasnoyarsk, Russia

I build AI-powered products end-to-end: from model selection and prompt engineering to production deployment with Docker.

## What I Do

- **RAG Systems** — LangChain, LlamaIndex, vector databases (PostgreSQL + pgvector)
- **LLM Integration** — API orchestration, prompt engineering, agent architectures
- **Telegram Bots** — aiogram 3, async Python, complex dialogue flows
- **Workflow Automation** — n8n, custom integrations, orchestrator patterns
- **Backend** — FastAPI, PostgreSQL, Docker, Linux

## Commercial Projects

Projects delivered for clients via freelance platforms.

**AI Consultant Chatbot for a Building Materials Store**
Self-hosted LLM platform with a product knowledge base, automated cost calculations, and a custom JS widget with SSE streaming deployed on the client's website.

**Stack:** Dify (self-hosted), Google Gemini, Docker, Nginx, JavaScript

**Gamification & AI Coach for a Health-Tech Telegram Bot**
Streak/milestone system with comeback detection, AI-powered personalized nutrition and fitness coaching with trial/paywall flow. Integrated into an existing production codebase via 17+ pull requests.

**Stack:** Python, aiogram 3, PostgreSQL, Redis, Docker, Alembic

## Featured Projects

### [sciwriter-mas](https://github.com/GleckusZeroFive/sciwriter-mas)
Multi-agent content generation pipeline with anti-hallucination system. Sectional Writer architecture (Planner → Section Writers → Assembler), deterministic fact validation, and dual-pass cleanup. Fact Precision ~80%.

**Stack:** CrewAI, LangGraph, PostgreSQL, Qdrant, Ollama, Docker

### [telegram-bot-templates](https://github.com/GleckusZeroFive/telegram-bot-templates)
RAG platform for Telegram — one Docker image, 5 products via YAML presets (HR, Support, Legal, Tutor, Voice). Hybrid search (BM25 + semantic + RRF), ONNX intent classifier (3.7ms), voice messages (Whisper STT).

**Stack:** Python, aiogram 3, Qdrant, Ollama, ONNX Runtime, Docker

### [intent-classifier](https://github.com/GleckusZeroFive/intent-classifier)
Fine-tuned ruBERT-tiny2 (29M params) for intent classification: rag/chat/followup. F1=0.90, 3.7ms inference on CPU. Published on HuggingFace, MIT license.

**Stack:** HuggingFace Transformers, ONNX Runtime, Google Colab

### [n8n-orchestrator-worker](https://github.com/GleckusZeroFive/n8n-orchestrator-worker)
Modular n8n automation system with Orchestrator + Worker architecture, NL intent detection, PostgreSQL session state (Supabase), and 3-level error handling with execution journal.

**Stack:** n8n, PostgreSQL, Supabase, Webhook API, JSON contracts

## Tech Stack

```
Python       | LangChain    | LlamaIndex   | FastAPI
aiogram 3    | asyncio      | PostgreSQL   | pgvector
Qdrant       | Docker       | Linux        | n8n
CrewAI       | LangGraph    | ONNX Runtime | Ollama
OpenAI API   | RAG          | NLP          | Prompt Engineering
```

## Contact

- **Kwork:** [gleckus19](https://kwork.ru/user/gleckus19)
- **Location:** Krasnoyarsk, Russia
