<div align="center">

<img src="assets/hero.svg" width="100%" alt="the-ai-stack"/>

<br/>

[![Stars](https://img.shields.io/github/stars/chitajohn/the-ai-stack?style=flat-square&color=111&labelColor=f0f0f0&label=stars)](https://github.com/chitajohn/the-ai-stack)
&nbsp;
![Updated](https://img.shields.io/badge/updated-2025-111?style=flat-square&labelColor=f0f0f0)
&nbsp;
![License](https://img.shields.io/badge/license-MIT-111?style=flat-square&labelColor=f0f0f0)
&nbsp;
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-111?style=flat-square&labelColor=f0f0f0)

</div>

---

## Navigate by Role

Organized around **who you are and what you need** — not an arbitrary category taxonomy.

| Role | What brings you here | Jump |
|------|----------------------|------|
| **Developer** | You're in the code. Pipelines, APIs, agents, infra, evals. | [Developers →](#developers) |
| **Founder / Builder** | You're shipping products. Speed, cost, and leverage matter most. | [Founders & Builders →](#founders--builders) |
| **Researcher** | Working at the model level — training, evaluating, publishing. | [Researchers →](#researchers) |
| **Everyone** | Start here to understand how all the pieces connect. | [Architecture →](#the-full-stack-architecture) |

---

## The Full Stack Architecture

<div align="center">
<img src="assets/architecture.svg" width="100%" alt="AI Stack Architecture Diagram"/>
</div>

<br/>

> Every tool in this repo maps to one of these five layers. Knowing the layer tells you what a tool *actually does* — independent of how it markets itself. When you encounter something new, the first question is always: which layer does this belong to?

---

## Developers

<img src="assets/banner-dev.svg" width="100%" alt="Developers"/>

<br/>

You're working at the layer where real engineering decisions get made — model selection, pipeline architecture, retrieval systems, agent design, deployment strategy. This section covers the full technical stack from raw API access to production observability.

<br/>

### Foundation Models & APIs

The raw intelligence layer. Everything else is built on top of these.

| Logo | Tool | What it actually is | Best for |
|------|------|---------------------|----------|
| <img src="https://cdn.simpleicons.org/openai/000000" width="18" height="18"/> | [**OpenAI**](https://platform.openai.com) | GPT-4o, o1, o3-mini — the API that normalized LLMs at scale | Broad use, function calling, Assistants API |
| <img src="https://cdn.simpleicons.org/anthropic/000000" width="18" height="18"/> | [**Anthropic**](https://console.anthropic.com) | Claude 3.5/3.7 Sonnet, Claude 3 Opus — alignment-first frontier lab | Long context, complex reasoning, agentic tool use |
| <img src="https://cdn.simpleicons.org/google/4285F4" width="18" height="18"/> | [**Google DeepMind**](https://aistudio.google.com) | Gemini 2.0 Flash, Pro, Ultra — natively multimodal from the ground up | Multimodal tasks, Google ecosystem integration |
| <img src="https://cdn.simpleicons.org/meta/0064e0" width="18" height="18"/> | [**Meta AI — Llama**](https://llama.meta.com) | Llama 3.3 70B, Llama 3.2 Vision — the open-weight family powering half the industry | Self-hosted deployments, fine-tuning, research |
| <img src="https://cdn.simpleicons.org/mistral/000000" width="18" height="18"/> | [**Mistral AI**](https://mistral.ai) | Mistral Large, Mixtral 8x22B MoE — high performance, EU-sovereign, genuinely open | Cost-efficient production, European data requirements |
| <img src="https://cdn.simpleicons.org/cohere/39594E" width="18" height="18"/> | [**Cohere**](https://cohere.com) | Command R+, Embed v3 — purpose-built for enterprise RAG and retrieval | Enterprise search pipelines, embeddings at scale |
| <img src="https://cdn.simpleicons.org/x/000000" width="18" height="18"/> | [**xAI — Grok**](https://x.ai) | Grok 3 — real-time web access baked in, strong at STEM | Real-time information, code, math-heavy tasks |
| <img src="https://cdn.simpleicons.org/amazonwebservices/FF9900" width="18" height="18"/> | [**Amazon Bedrock**](https://aws.amazon.com/bedrock) | Managed access to Claude, Titan, Llama, Mistral, and more via AWS | Multi-model enterprise workloads on AWS |
| <img src="https://cdn.simpleicons.org/deepseek/4D6BFF" width="18" height="18"/> | [**DeepSeek**](https://deepseek.com) | DeepSeek R1, V3 — open reasoning models competitive with o1 at a fraction of the cost | Cost-efficient reasoning, open-weight flexibility |
| <img src="https://cdn.simpleicons.org/huggingface/FFD21E" width="18" height="18"/> | [**Hugging Face**](https://huggingface.co) | The central hub for everything open — models, datasets, spaces, inference | Open-source model access, community models |

<br/>

### Inference & Speed

A model is only as useful as it is fast enough for your product's latency floor.

| Logo | Tool | What it does | Why it matters |
|------|------|--------------|----------------|
| <img src="https://cdn.simpleicons.org/groq/F55036" width="18" height="18"/> | [**Groq**](https://groq.com) | LPU-based inference — Llama, Mixtral, Gemma at speeds that feel instant | The current benchmark for open model inference speed |
| <img src="https://cdn.simpleicons.org/cloudflare/F38020" width="18" height="18"/> | [**Cloudflare Workers AI**](https://developers.cloudflare.com/workers-ai) | Serverless inference at the edge — zero cold starts, globally distributed | Edge AI, latency-sensitive global applications |
| <img src="https://cdn.simpleicons.org/amazonwebservices/FF9900" width="18" height="18"/> | [**AWS SageMaker**](https://aws.amazon.com/sagemaker) | Fully managed ML platform — train, deploy, and monitor at enterprise scale | Organizations already running deep in the AWS ecosystem |
| <img src="https://cdn.simpleicons.org/huggingface/FFD21E" width="18" height="18"/> | [**HF Inference Endpoints**](https://huggingface.co/inference-endpoints) | One-click private deployment for any HuggingFace model | Fastest path from model card to production API |
| <img src="https://cdn.simpleicons.org/pytorch/EE4C2C" width="18" height="18"/> | [**vLLM**](https://github.com/vllm-project/vllm) | PagedAttention-based high-throughput inference for self-hosted models | Maximum throughput on self-hosted open models |
| <img src="https://cdn.simpleicons.org/ollama/000000" width="18" height="18"/> | [**Ollama**](https://ollama.com) | Pull and run any open model locally with a single command | Local development, air-gapped environments, zero API cost |
| <img src="https://cdn.simpleicons.org/together/000000" width="18" height="18"/> | [**Together AI**](https://www.together.ai) | Run and fine-tune open models on shared GPU infrastructure | Production open-model workloads with fine-tune capability |

<br/>

### Frameworks & Orchestration

Single API calls build demos. Frameworks build products.

| Logo | Tool | Architecture | Strengths |
|------|------|--------------|-----------|
| <img src="https://cdn.simpleicons.org/langchain/1C3C3C" width="18" height="18"/> | [**LangChain**](https://www.langchain.com) | Chain-based, component-driven | Most widely adopted, massive ecosystem, deep integrations |
| <img src="https://cdn.simpleicons.org/llamaindex/000000" width="18" height="18"/> | [**LlamaIndex**](https://www.llamaindex.ai) | Data-centric, retrieval-first | Best-in-class data ingestion and structured indexing for RAG |
| <img src="https://cdn.simpleicons.org/microsoft/512BD4" width="18" height="18"/> | [**Semantic Kernel**](https://github.com/microsoft/semantic-kernel) | Plugin architecture | .NET and Python, Microsoft ecosystem, enterprise-grade |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**DSPy**](https://github.com/stanfordnlp/dspy) | Declarative, compile-to-prompt | Program LLM pipelines algorithmically — no manual prompt writing |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Haystack**](https://haystack.deepset.ai) | Pipeline DAG | Production NLP pipelines, strong for search and QA systems |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Instructor**](https://github.com/jxnl/instructor) | Pydantic-native structured outputs | Force any LLM to return typed, validated data structures reliably |
| <img src="https://cdn.simpleicons.org/flowise/1CC886" width="18" height="18"/> | [**Flowise**](https://flowiseai.com) | Visual drag-and-drop | Build LLM pipelines without writing orchestration code |
| <img src="https://cdn.simpleicons.org/dify/000000" width="18" height="18"/> | [**Dify**](https://dify.ai) | Full LLMOps platform | No-code pipeline builder + API + observability in one platform |

<br/>

### RAG & Memory

Context determines capability. These give your models what they cannot know from training alone.

| Logo | Tool | Type | Notes |
|------|------|------|-------|
| <img src="https://cdn.simpleicons.org/pinecone/000000" width="18" height="18"/> | [**Pinecone**](https://www.pinecone.io) | Managed vector DB | The production standard for managed vector search at scale |
| <img src="https://cdn.simpleicons.org/chroma/FF6B35" width="18" height="18"/> | [**Chroma**](https://www.trychroma.com) | Open-source vector DB | Fastest path from dev to prototype — fully self-hostable |
| <img src="https://cdn.simpleicons.org/weaviate/00C5A8" width="18" height="18"/> | [**Weaviate**](https://weaviate.io) | Open-source vector DB | Hybrid search (dense + sparse), strong GraphQL interface |
| <img src="https://cdn.simpleicons.org/qdrant/DC244C" width="18" height="18"/> | [**Qdrant**](https://qdrant.tech) | Open-source vector DB | High performance, rich payload filtering, Rust-native speed |
| <img src="https://cdn.simpleicons.org/redis/FF4438" width="18" height="18"/> | [**Redis Stack**](https://redis.io/docs/latest/develop/get-started/vector-database) | In-memory vector DB | Vector search on infrastructure you likely already run |
| <img src="https://cdn.simpleicons.org/postgresql/336791" width="18" height="18"/> | [**pgvector**](https://github.com/pgvector/pgvector) | Postgres extension | Vector search inside existing Postgres — zero new infrastructure |
| <img src="https://cdn.simpleicons.org/mongodb/47A248" width="18" height="18"/> | [**MongoDB Atlas Vector**](https://www.mongodb.com/products/platform/atlas-vector-search) | Managed vector DB | Vector search layered directly onto existing MongoDB collections |
| <img src="https://cdn.simpleicons.org/mem0/000000" width="18" height="18"/> | [**Mem0**](https://mem0.ai) | Memory layer | Persistent cross-session memory for assistants and agents |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Zep**](https://getzep.com) | Memory layer | Long-term conversational memory with automatic entity extraction |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**LightRAG**](https://github.com/HKUDS/LightRAG) | Graph-based RAG | Knowledge graph retrieval — better than naive chunking for connected data |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Ragie**](https://ragie.ai) | Managed RAG | Fully managed RAG pipeline — ingest, chunk, embed, retrieve as a service |

<br/>

### Agents & Tool Use

The shift from generation to execution. Models that don't just respond — they act.

| Logo | Tool | Paradigm | Core capability |
|------|------|----------|----------------|
| <img src="https://cdn.simpleicons.org/openai/000000" width="18" height="18"/> | [**OpenAI Agents SDK**](https://github.com/openai/openai-agents-python) | Single + multi-agent | Official lightweight framework — handoffs, tools, guardrails, built-in tracing |
| <img src="https://cdn.simpleicons.org/microsoft/512BD4" width="18" height="18"/> | [**AutoGen**](https://github.com/microsoft/autogen) | Multi-agent conversation | Agents that collaborate with each other to solve complex tasks |
| <img src="https://cdn.simpleicons.org/crewai/000000" width="18" height="18"/> | [**CrewAI**](https://www.crewai.com) | Role-based multi-agent | Specialized agents with defined roles, tasks, and inter-agent delegation |
| <img src="https://cdn.simpleicons.org/langchain/1C3C3C" width="18" height="18"/> | [**LangGraph**](https://github.com/langchain-ai/langgraph) | Graph-based agent flows | Stateful, cyclical agent execution — built for complex agent orchestration |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Browser Use**](https://github.com/browser-use/browser-use) | Browser automation | Give any LLM full browser control with structured action output |
| <img src="https://cdn.simpleicons.org/anthropic/000000" width="18" height="18"/> | [**Claude Computer Use**](https://docs.anthropic.com/en/docs/agents-and-tools/computer-use) | Desktop-level control | Anthropic's API for full OS-level agent interaction |
| <img src="https://cdn.simpleicons.org/e2b/000000" width="18" height="18"/> | [**E2B**](https://e2b.dev) | Sandboxed code execution | Secure, isolated execution environments for agent-generated code |
| <img src="https://cdn.simpleicons.org/composio/000000" width="18" height="18"/> | [**Composio**](https://composio.dev) | Tool integrations | 250+ pre-built integrations for agents — one unified SDK |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Firecrawl**](https://firecrawl.dev) | Web data extraction | Turn any website into structured, LLM-ready data via API |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Phidata**](https://www.phidata.com) | Agentic app platform | Build, ship, and monitor agentic applications end-to-end |

<br/>

### Evals & Testing

Ship with confidence. "It seemed to work in the demo" is not a quality bar.

| Logo | Tool | Eval scope |
|------|------|------------|
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Promptfoo**](https://www.promptfoo.dev) | Prompt comparison, regression testing, adversarial red-teaming — CLI-first |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**DeepEval**](https://github.com/confident-ai/deepeval) | 14+ LLM-specific metrics — hallucination, faithfulness, relevance, toxicity |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**RAGAS**](https://ragas.io) | RAG-specific evaluation — context precision, recall, faithfulness |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Braintrust**](https://www.braintrustdata.com) | Full-cycle eval — scoring, logging, prompt versioning, regression CI |
| <img src="https://cdn.simpleicons.org/openai/000000" width="18" height="18"/> | [**OpenAI Evals**](https://github.com/openai/evals) | Open-source framework for evaluating LLM completions at scale |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Giskard**](https://www.giskard.ai) | LLM vulnerability scanning — bias, hallucination, prompt injection detection |
| <img src="https://cdn.simpleicons.org/cometml/FF6F61" width="18" height="18"/> | [**Opik**](https://www.comet.com/site/products/opik) | Open-source eval and observability platform from Comet ML |

<br/>

### Observability & Monitoring

You cannot improve what you cannot see. Production AI demands production-grade visibility.

| Logo | Tool | Coverage |
|------|------|----------|
| <img src="https://cdn.simpleicons.org/langfuse/000000" width="18" height="18"/> | [**Langfuse**](https://langfuse.com) | Open-source tracing, analytics, and prompt management — self-hostable |
| <img src="https://cdn.simpleicons.org/langchain/1C3C3C" width="18" height="18"/> | [**LangSmith**](https://www.langsmith.com) | Deep tracing and debugging native to LangChain-based applications |
| <img src="https://cdn.simpleicons.org/helicone/FF6B35" width="18" height="18"/> | [**Helicone**](https://www.helicone.ai) | One-line proxy — logs every LLM call across every provider automatically |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Arize AI**](https://arize.com) | Full ML and LLM observability with drift detection and alerting |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Portkey**](https://portkey.ai) | AI gateway with load balancing, caching, fallbacks, and budget controls |
| <img src="https://cdn.simpleicons.org/weightsandbiases/FFBE00" width="18" height="18"/> | [**Weights & Biases**](https://wandb.ai) | The ML experiment tracker — now with full LLM tracing and eval support |

<br/>

### Deployment & Serving

Moving from a prototype to infrastructure other people can rely on.

| Logo | Tool | Deploy model |
|------|------|--------------|
| <img src="https://cdn.simpleicons.org/modal/000000" width="18" height="18"/> | [**Modal**](https://modal.com) | Serverless GPU workloads — deploy ML functions with zero infra management |
| <img src="https://cdn.simpleicons.org/vercel/000000" width="18" height="18"/> | [**Vercel AI SDK**](https://sdk.vercel.ai) | First-class streaming AI responses for Next.js and any web framework |
| <img src="https://cdn.simpleicons.org/pytorch/EE4C2C" width="18" height="18"/> | [**vLLM**](https://github.com/vllm-project/vllm) | PagedAttention-based high-throughput inference engine for self-hosted models |
| <img src="https://cdn.simpleicons.org/bentoml/000000" width="18" height="18"/> | [**BentoML**](https://www.bentoml.com) | Package any ML model into a production-grade service with one CLI command |
| <img src="https://cdn.simpleicons.org/ray/028CF0" width="18" height="18"/> | [**Ray Serve**](https://docs.ray.io/en/latest/serve) | Distributed model serving on Ray — horizontal scaling by default |
| <img src="https://cdn.simpleicons.org/amazonwebservices/FF9900" width="18" height="18"/> | [**SageMaker Inference**](https://aws.amazon.com/sagemaker/deploy) | Managed endpoints with autoscaling on AWS |
| <img src="https://cdn.simpleicons.org/huggingface/FFD21E" width="18" height="18"/> | [**HF Inference Endpoints**](https://huggingface.co/inference-endpoints) | One-click private deployment for any HuggingFace model |

<br/>

### Developer Tooling

The local environment stack that makes you measurably faster.

| Logo | Tool | What it changes |
|------|------|-----------------|
| <img src="https://cdn.simpleicons.org/anthropic/000000" width="18" height="18"/> | [**Claude Code**](https://claude.ai/code) | Agentic, terminal-native coding — reads your codebase, writes, tests, commits |
| <img src="https://cdn.simpleicons.org/cursor/000000" width="18" height="18"/> | [**Cursor**](https://www.cursor.com) | The IDE rebuilt around AI — codebase-aware edits, multi-file reasoning |
| <img src="https://cdn.simpleicons.org/github/181717" width="18" height="18"/> | [**GitHub Copilot**](https://github.com/features/copilot) | The most widely deployed AI coding assistant — deeply integrated into GitHub |
| <img src="https://cdn.simpleicons.org/codeium/09B37B" width="18" height="18"/> | [**Codeium**](https://codeium.com) | Free AI autocomplete and chat across 70+ languages |
| <img src="https://cdn.simpleicons.org/visualstudiocode/007ACC" width="18" height="18"/> | [**Continue**](https://www.continue.dev) | Open-source AI code assistant for VS Code and JetBrains — bring any model |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Aider**](https://aider.chat) | AI pair programmer that works inside your terminal with native git integration |
| <img src="https://cdn.simpleicons.org/codeium/09B37B" width="18" height="18"/> | [**Windsurf**](https://codeium.com/windsurf) | Codeium's AI-native IDE — Cascade engine handles multi-step agentic implementation |

---

## Founders & Builders

<img src="assets/banner-founders.svg" width="100%" alt="Founders and Builders"/>

<br/>

You're not building the AI — you're building *with* it. Speed, cost, and product leverage matter more than architectural purity. This section is organized around decisions you actually face: how to prototype before you commit, which infrastructure to trust with production traffic, how to control costs as you scale.

<br/>

### Prototype-to-Product Stack

The fastest path from a validated idea to something that actually works.

| Logo | Tool | What it generates | Ships? |
|------|------|-------------------|--------|
| <img src="https://cdn.simpleicons.org/vercel/000000" width="18" height="18"/> | [**v0 by Vercel**](https://v0.dev) | Full React/shadcn components from a text description | Deploys to Vercel |
| <img src="https://cdn.simpleicons.org/stackblitz/1389FD" width="18" height="18"/> | [**Bolt.new**](https://bolt.new) | Full-stack apps in the browser — frontend, backend, database in one session | One-click deploy |
| <img src="https://cdn.simpleicons.org/supabase/3ECF8E" width="18" height="18"/> | [**Lovable**](https://lovable.dev) | AI-generated full-stack web apps with visual editor and Supabase integration | One-click deploy |
| <img src="https://cdn.simpleicons.org/replit/F26207" width="18" height="18"/> | [**Replit Agent**](https://replit.com/ai) | Build, run, and host apps entirely inside Replit — zero local setup | Runs on Replit |
| <img src="https://cdn.simpleicons.org/cursor/000000" width="18" height="18"/> | [**Cursor**](https://www.cursor.com) | Write production-grade code faster than any current alternative | Manual |
| <img src="https://cdn.simpleicons.org/codeium/09B37B" width="18" height="18"/> | [**Windsurf**](https://codeium.com/windsurf) | Agentic IDE — Cascade handles multi-step implementation from a single instruction | Manual |

<br/>

### AI-Powered Product Infrastructure

The APIs and platforms that power what your users actually experience.

| Logo | Tool | Core offering | What it powers in your product |
|------|------|---------------|--------------------------------|
| <img src="https://cdn.simpleicons.org/openai/000000" width="18" height="18"/> | [**OpenAI Platform**](https://platform.openai.com) | Assistants API, Realtime API, function calling, file search | Chatbots, voice interfaces, document Q&A |
| <img src="https://cdn.simpleicons.org/anthropic/000000" width="18" height="18"/> | [**Anthropic API**](https://console.anthropic.com) | Claude API — tool use, long documents, computer use | Complex reasoning, document processing, agentic features |
| <img src="https://cdn.simpleicons.org/vercel/000000" width="18" height="18"/> | [**Vercel AI SDK**](https://sdk.vercel.ai) | Streaming AI in any web framework — React, Next.js, SvelteKit | Real-time streaming responses in any web product |
| <img src="https://cdn.simpleicons.org/supabase/3ECF8E" width="18" height="18"/> | [**Supabase**](https://supabase.com) | Postgres + pgvector + auth + storage + realtime — the complete backend | Full backend for AI-powered web and mobile apps |
| <img src="https://cdn.simpleicons.org/firebase/FFCA28" width="18" height="18"/> | [**Firebase + Vertex AI**](https://firebase.google.com/products/vertex-ai) | Gemini in Firebase — auth, storage, and AI in one SDK | Mobile and web apps with native Google AI integration |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**LiteLLM**](https://litellm.ai) | Unified API across 100+ models — one interface, every provider | Vendor flexibility, cost routing, fallback logic |
| <img src="https://cdn.simpleicons.org/openrouter/000000" width="18" height="18"/> | [**OpenRouter**](https://openrouter.ai) | Route requests to the best model for your cost and quality threshold | Dynamic cost optimization across model providers |

<br/>

### Voice, Multimodal & Media Generation

Beyond text — products that see, hear, speak, and create.

| Logo | Tool | Modality | Production status |
|------|------|----------|-------------------|
| <img src="https://cdn.simpleicons.org/elevenlabs/000000" width="18" height="18"/> | [**ElevenLabs**](https://elevenlabs.io) | TTS, voice cloning, AI dubbing | Production — highest output quality available |
| <img src="https://cdn.simpleicons.org/openai/000000" width="18" height="18"/> | [**OpenAI Whisper**](https://github.com/openai/whisper) | Speech-to-text — open-source, multilingual, highly accurate | Production — self-host or use via API |
| <img src="https://cdn.simpleicons.org/assemblyai/000000" width="18" height="18"/> | [**AssemblyAI**](https://www.assemblyai.com) | STT with LLM intelligence — summaries, entities, sentiment baked in | Production — API-first, generous feature set |
| <img src="https://cdn.simpleicons.org/fal/000000" width="18" height="18"/> | [**fal.ai**](https://fal.ai) | Fast inference for FLUX, Stable Diffusion, video models | Production — fastest image generation API |
| <img src="https://cdn.simpleicons.org/runway/000000" width="18" height="18"/> | [**Runway**](https://runwayml.com) | AI video generation and editing — Gen-3 Alpha | Production — the creative professional's standard |
| <img src="https://cdn.simpleicons.org/openai/000000" width="18" height="18"/> | [**Sora**](https://sora.com) | OpenAI's video generation — cinematic quality from text or image | Production — API via OpenAI |
| <img src="https://cdn.simpleicons.org/roboflow/purple" width="18" height="18"/> | [**Roboflow**](https://roboflow.com) | Computer vision platform — train and deploy vision models end-to-end | Production — strongest CV builder ecosystem |
| <img src="https://cdn.simpleicons.org/stability/000000" width="18" height="18"/> | [**Stability AI**](https://stability.ai) | Stable Diffusion open-source image generation models | Production — open-weight image generation |

<br/>

### Cost Management & Model Routing

Because the infrastructure bill is always somebody's responsibility.

| Logo | Tool | What it controls |
|------|------|-----------------|
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**LiteLLM**](https://litellm.ai) | Single unified API for any provider — swap models without changing code |
| <img src="https://cdn.simpleicons.org/openrouter/000000" width="18" height="18"/> | [**OpenRouter**](https://openrouter.ai) | Automatic routing to the cheapest model meeting your quality threshold |
| <img src="https://cdn.simpleicons.org/helicone/FF6B35" width="18" height="18"/> | [**Helicone**](https://www.helicone.ai) | Real-time spend tracking, latency analytics, prompt caching insights |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Portkey**](https://portkey.ai) | Gateway with load balancing, caching, fallbacks, and hard budget limits |

<br/>

### No-Code & Low-Code AI

Real leverage without writing orchestration code.

| Logo | Tool | What you can build |
|------|------|-------------------|
| <img src="https://cdn.simpleicons.org/zapier/FF4A00" width="18" height="18"/> | [**Zapier AI**](https://zapier.com/ai) | AI-powered automations across 7,000+ apps — pure no-code |
| <img src="https://cdn.simpleicons.org/make/6D00CC" width="18" height="18"/> | [**Make**](https://make.com) | Visual workflow automation with AI module support — more power than Zapier |
| <img src="https://cdn.simpleicons.org/flowise/1CC886" width="18" height="18"/> | [**Flowise**](https://flowiseai.com) | Open-source drag-and-drop LLM app builder — fully self-hostable |
| <img src="https://cdn.simpleicons.org/dify/000000" width="18" height="18"/> | [**Dify**](https://dify.ai) | Full LLMOps platform — visual builder, API, versioning, observability |
| <img src="https://cdn.simpleicons.org/n8n/EA4B71" width="18" height="18"/> | [**n8n**](https://n8n.io) | Self-hostable workflow automation with AI nodes and code escapes |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Relevance AI**](https://relevanceai.com) | Build AI agents and tools without code — deploy as production APIs |

---

## Researchers

<img src="assets/banner-researchers.svg" width="100%" alt="Researchers"/>

<br/>

You're not consuming what exists — you're evaluating it, pushing against it, and extending it. This section covers the open model ecosystem, the fine-tuning toolchain, the benchmarks that carry actual signal, and the literature worth reading from first principles.

<br/>

### Open Models & Weights

The open-weight ecosystem has matured to the point where, for most tasks, the capability gap with proprietary models is negligible or closed.

| Model | Org | Params | What sets it apart |
|-------|-----|--------|-------------------|
| [**Llama 3.3 70B**](https://llama.meta.com) | Meta | 70B | Reference open model — strongest general-purpose at its size class |
| [**Llama 3.2 Vision**](https://llama.meta.com) | Meta | 11B–90B | Multimodal open model — image understanding at scale |
| [**Mixtral 8x22B**](https://mistral.ai/models) | Mistral | 141B MoE | Sparse MoE — frontier capability at reduced inference cost |
| [**Mistral Small 3**](https://mistral.ai/models) | Mistral | 24B | Highest performance-per-parameter in the sub-30B class |
| [**DeepSeek R1**](https://deepseek.com) | DeepSeek | 671B MoE | Open reasoning model — genuinely competitive with o1 on math and code |
| [**DeepSeek V3**](https://deepseek.com) | DeepSeek | 685B MoE | Frontier-level open model at accessible inference cost |
| [**Qwen 2.5 72B**](https://qwenlm.github.io) | Alibaba | 72B | Exceptional multilingual, coding, and mathematics performance |
| [**Qwen 2.5 Coder**](https://qwenlm.github.io) | Alibaba | 32B | The strongest open-weight coding model currently available |
| [**Gemma 3**](https://ai.google.dev/gemma) | Google | 1B–27B | Lightweight, Apache 2.0, optimized for research and edge deployment |
| [**Phi-4**](https://huggingface.co/microsoft/phi-4) | Microsoft | 14B | Punches well above its weight class on reasoning benchmarks |
| [**Command R+**](https://cohere.com/command) | Cohere | 104B | Purpose-built for RAG and enterprise tool use |

<br/>

### Fine-tuning & Adaptation

Making a general model genuinely capable at your specific problem domain.

| Logo | Tool | Approach | When to reach for it |
|------|------|----------|----------------------|
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Unsloth**](https://github.com/unslothai/unsloth) | Optimized training kernels | 2× faster, 70% less VRAM — the default for local fine-tuning |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**Axolotl**](https://github.com/axolotl-ai-cloud/axolotl) | Config-driven | Streamlined fine-tuning with broad architecture and dataset format support |
| <img src="https://cdn.simpleicons.org/python/3776AB" width="18" height="18"/> | [**LLaMA-Factory**](https://github.com/hiyouga/LLaMA-Factory) | Unified framework | Fine-tune 100+ model families from one standardized interface |
| <img src="https://cdn.simpleicons.org/huggingface/FFD21E" width="18" height="18"/> | [**HuggingFace TRL**](https://github.com/huggingface/trl) | RLHF toolkit | The standard library for SFT, RLHF, DPO, and PPO training |
| <img src="https://cdn.simpleicons.org/openai/000000" width="18" height="18"/> | [**OpenAI Fine-tuning**](https://platform.openai.com/docs/guides/fine-tuning) | Managed service | Managed SFT for GPT-4o mini — no infrastructure to manage |
| <img src="https://cdn.simpleicons.org/microsoft/512BD4" width="18" height="18"/> | [**LoRA / QLoRA**](https://github.com/microsoft/LoRA) | Parameter-efficient | Adapt large models on consumer hardware with minimal parameter overhead |

<br/>

### Benchmarks That Actually Matter

The only evaluations worth tracking are ones that cannot be gamed through memorization.

| Benchmark | What it actually tests | Org |
|-----------|------------------------|-----|
| [**MMLU**](https://github.com/hendrycks/test) | Knowledge across 57 academic subjects — STEM to law | UC Berkeley |
| [**HumanEval**](https://github.com/openai/human-eval) | Code generation — function completion from docstrings | OpenAI |
| [**MATH**](https://github.com/hendrycks/math) | Competition-level mathematics — AMC, AIME, algebra, combinatorics | UC Berkeley |
| [**HELM**](https://crfm.stanford.edu/helm) | Holistic evaluation — accuracy, calibration, robustness, fairness | Stanford CRFM |
| [**BIG-Bench Hard**](https://github.com/suzgunmirac/BIG-Bench-Hard) | 23 tasks that consistently stumped prior model generations | Google |
| [**LMSYS Chatbot Arena**](https://chat.lmsys.org) | Human preference via blind pairwise comparison — the most credible leaderboard | LMSYS |
| [**LiveBench**](https://livebench.ai) | Contamination-free — new questions sourced monthly from recent data | Independent |
| [**SWE-Bench**](https://www.swebench.com) | Real GitHub software engineering issues — the coding benchmark that matters | Princeton |
| [**GPQA**](https://github.com/idavidrein/gpqa) | Expert-level biology, chemistry, physics — PhD-level difficulty | NYU |

<br/>

### Essential Reading

Papers and resources that provide genuine understanding — not surface familiarity with the vocabulary.

**Foundational**

| Paper | Why it earns its place |
|-------|------------------------|
| [Attention Is All You Need (2017)](https://arxiv.org/abs/1706.03762) | The transformer paper — every current architecture descends from this |
| [Scaling Laws for Neural LMs (2020)](https://arxiv.org/abs/2001.08361) | The mathematical relationship between compute, data, and capability |
| [InstructGPT (2022)](https://arxiv.org/abs/2203.02155) | How RLHF made GPT-3 usable — the alignment paper that shipped |
| [Constitutional AI (2022)](https://arxiv.org/abs/2212.08073) | Anthropic's alignment approach — the technical basis for Claude |

**Architecture & efficiency**

| Paper | Why it earns its place |
|-------|------------------------|
| [LoRA (2021)](https://arxiv.org/abs/2106.09685) | Low-rank adaptation — fine-tuning tractable on consumer hardware |
| [Flash Attention (2022)](https://arxiv.org/abs/2205.14135) | The engineering advance that unlocked long context windows |
| [Chain-of-Thought Prompting (2022)](https://arxiv.org/abs/2201.11903) | Why explicit reasoning steps improve outputs — and the mechanism behind it |
| [Mixture of Experts Survey](https://arxiv.org/abs/2209.01667) | The architecture behind Mixtral, GPT-4, and DeepSeek |

**Retrieval & memory**

| Paper | Why it earns its place |
|-------|------------------------|
| [RAG (2020)](https://arxiv.org/abs/2005.11401) | The original paper unifying retrieval with generation |
| [Lost in the Middle (2023)](https://arxiv.org/abs/2307.03172) | Why LLMs miss information placed in the middle of long contexts |

**Explainers worth bookmarking**

| Resource | What it gives you |
|----------|------------------|
| [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer) | The definitive visual walkthrough of transformer internals |
| [Andrej Karpathy — Zero to Hero](https://karpathy.ai/zero-to-hero.html) | Build everything from scratch — the most thorough practical curriculum available |
| [Anthropic Interpretability Research](https://www.anthropic.com/research) | Mechanistic interpretability — what is actually inside these models |
| [Lilian Weng's Blog](https://lilianweng.github.io) | Deep, consistently accurate writing on agents, alignment, and training methods |

---

## Contributing

This is a living reference. If something belongs here and isn't here yet, a PR is the right move.

**The bar for inclusion:**
- Actively maintained and publicly accessible
- Serves a real, distinct function — not a rebrand of an existing capability
- Maps clearly to one of the five architectural layers
- One sentence is sufficient to describe what it does

**Format:** Match the table structure and logo style of the section you're adding to. Place the tool in the correct layer, not just the most visible section.

---

<div align="center">

<br/>

Maintained by &nbsp;[![Follow on X](https://img.shields.io/badge/@chitajohn__-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/chitajohn_)

<br/>

*If this reference saved you time — share it with someone building something worth building.*

[MIT License](LICENSE)

</div>
