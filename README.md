<div align="center">

![the-ai-stack](./assets/hero.svg)

<br/>

**One repo to understand the entire AI stack.**  
Organized by role. Curated with intent. No filler.

<br/>

![GitHub Stars](https://img.shields.io/github/stars/chitajohn/the-ai-stack?style=flat-square&color=111111&labelColor=fafafa)
![Last Updated](https://img.shields.io/badge/updated-2025-111111?style=flat-square&labelColor=fafafa)
![Open Source](https://img.shields.io/badge/open--source-yes-111111?style=flat-square&labelColor=fafafa)

</div>

---

## How to navigate

This repo is organized by **role**, not by category. Jump to what applies to you.

| I am a... | Go to |
|-----------|-------|
| 🧑‍💻 Developer building AI-powered products | [→ Developers](#-developers) |
| 🏗️ Founder or builder shipping with AI | [→ Founders & Builders](#️-founders--builders) |
| 🔬 Researcher working with models | [→ Researchers](#-researchers) |
| 🗺️ Just want to understand the landscape | [→ Architecture](#-the-ai-stack-architecture) |

---

## 🗺 The AI Stack — Architecture

![Architecture Diagram](./assets/architecture.svg)

> Every tool in this repo maps to one of these five layers.  
> Knowing the layer tells you what a tool *actually does* — not just what it markets itself as.

---

## 🧑‍💻 Developers

![Developers Banner](./assets/banner-dev.svg)

You're building AI-powered products. APIs, pipelines, RAG systems, agents. This section covers the full technical stack from model access to production deployment.

<br/>

### Foundation Models & APIs

The raw intelligence. Everything runs on top of these.

| Tool | Layer | What it actually is |
|------|-------|---------------------|
| [![OpenAI](https://img.shields.io/badge/OpenAI-000000?style=flat-square&logo=openai&logoColor=white)](https://platform.openai.com) | Models | GPT-4o, o1, o3 — the API that normalized LLMs at scale |
| [![Anthropic](https://img.shields.io/badge/Anthropic-000000?style=flat-square)](https://console.anthropic.com) | Models | Claude 3.5/3.7 — strongest at long context, reasoning, and instruction-following |
| [![Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=flat-square&logo=google&logoColor=white)](https://aistudio.google.com) | Models | Gemini 2.0 — natively multimodal, deep Google integration |
| [![Mistral](https://img.shields.io/badge/Mistral_AI-000000?style=flat-square)](https://mistral.ai) | Models | Open-weight and API — efficient, fast, capable, EU-based |
| [![Cohere](https://img.shields.io/badge/Cohere-000000?style=flat-square)](https://cohere.com) | Models | Enterprise-grade embeddings and generation |
| [![Meta Llama](https://img.shields.io/badge/Meta_Llama-0064e0?style=flat-square&logo=meta&logoColor=white)](https://llama.meta.com) | Models | Open-weight family — the backbone of self-hosted AI |
| [![xAI Grok](https://img.shields.io/badge/xAI_Grok-000000?style=flat-square)](https://x.ai) | Models | Grok 3 — real-time web access, strong STEM reasoning |

<br/>

### Inference & Speed

Models are only useful if they're fast enough for your product.

| Tool | What it does |
|------|--------------|
| [![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square)](https://groq.com) | LPU-based inference — runs open models at speeds that feel instant |
| [![Together AI](https://img.shields.io/badge/Together_AI-000000?style=flat-square)](https://www.together.ai) | Run and fine-tune open-source models on shared infra |
| [![Fireworks AI](https://img.shields.io/badge/Fireworks_AI-FF6B35?style=flat-square)](https://fireworks.ai) | Fast inference API for open models, compound AI systems |
| [![Cerebras](https://img.shields.io/badge/Cerebras-000000?style=flat-square)](https://cerebras.ai) | Wafer-scale chips — absurd tokens/second for large models |
| [![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square)](https://ollama.com) | Run any open model locally — no setup friction |

<br/>

### Frameworks & Orchestration

Single API calls won't build products. These make pipelines possible.

| Tool | Strength |
|------|----------|
| [![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)](https://www.langchain.com) | The most adopted framework — chains, tools, memory, agents |
| [![LlamaIndex](https://img.shields.io/badge/LlamaIndex-000000?style=flat-square)](https://www.llamaindex.ai) | Data ingestion and retrieval-first architecture |
| [![DSPy](https://img.shields.io/badge/DSPy-000000?style=flat-square)](https://github.com/stanfordnlp/dspy) | Program LLM pipelines instead of prompting them |
| [![Haystack](https://img.shields.io/badge/Haystack-00C5A8?style=flat-square)](https://haystack.deepset.ai) | Production NLP pipelines for search and QA |
| [![Semantic Kernel](https://img.shields.io/badge/Semantic_Kernel-512BD4?style=flat-square&logo=microsoft)](https://github.com/microsoft/semantic-kernel) | Microsoft's SDK — .NET and Python, enterprise focus |

<br/>

### RAG & Memory

Context is everything. These give models what they can't know by default.

| Tool | Type | Notes |
|------|------|-------|
| [![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square)](https://www.pinecone.io) | Managed Vector DB | Easiest path to production-grade vector search |
| [![Chroma](https://img.shields.io/badge/Chroma-FF6B35?style=flat-square)](https://www.trychroma.com) | Open-source Vector DB | Best for local dev and prototyping |
| [![Weaviate](https://img.shields.io/badge/Weaviate-00C5A8?style=flat-square)](https://weaviate.io) | Open-source Vector DB | Hybrid search — dense + sparse retrieval |
| [![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square)](https://qdrant.tech) | Open-source Vector DB | High-performance with rich filtering |
| [![pgvector](https://img.shields.io/badge/pgvector-336791?style=flat-square&logo=postgresql&logoColor=white)](https://github.com/pgvector/pgvector) | Postgres Extension | Vector search inside your existing Postgres — no new infra |
| [![Mem0](https://img.shields.io/badge/Mem0-000000?style=flat-square)](https://mem0.ai) | Memory Layer | Persistent memory for AI assistants and agents |
| [![Zep](https://img.shields.io/badge/Zep-000000?style=flat-square)](https://getzep.com) | Memory Layer | Long-term memory for conversational agents |

<br/>

### Agents & Tool Use

Models that act, not just generate.

| Tool | What it enables |
|------|-----------------|
| [![OpenAI Agents SDK](https://img.shields.io/badge/OpenAI_Agents_SDK-000000?style=flat-square&logo=openai&logoColor=white)](https://github.com/openai/openai-agents-python) | Lightweight official framework — handoffs, tools, guardrails |
| [![AutoGen](https://img.shields.io/badge/AutoGen-512BD4?style=flat-square&logo=microsoft)](https://github.com/microsoft/autogen) | Multi-agent conversations — agents that talk to each other |
| [![CrewAI](https://img.shields.io/badge/CrewAI-DC244C?style=flat-square)](https://www.crewai.com) | Role-based multi-agent teams with defined workflows |
| [![Browser Use](https://img.shields.io/badge/Browser_Use-000000?style=flat-square)](https://github.com/browser-use/browser-use) | Give agents full browser control |
| [![Claude Computer Use](https://img.shields.io/badge/Claude_Computer_Use-000000?style=flat-square)](https://docs.anthropic.com/en/docs/agents-and-tools/computer-use) | Anthropic's API for desktop-level agent control |
| [![E2B](https://img.shields.io/badge/E2B-000000?style=flat-square)](https://e2b.dev) | Sandboxed code execution environments for agents |
| [![Composio](https://img.shields.io/badge/Composio-000000?style=flat-square)](https://composio.dev) | 250+ tool integrations for agents — one SDK |

<br/>

### Evals & Testing

Vibes are not a benchmark.

| Tool | What it covers |
|------|----------------|
| [![Promptfoo](https://img.shields.io/badge/Promptfoo-000000?style=flat-square)](https://www.promptfoo.dev) | Prompt testing, comparison, and red-teaming from CLI |
| [![DeepEval](https://img.shields.io/badge/DeepEval-000000?style=flat-square)](https://github.com/confident-ai/deepeval) | Open-source eval framework — 14+ LLM metrics out of the box |
| [![RAGAS](https://img.shields.io/badge/RAGAS-000000?style=flat-square)](https://ragas.io) | RAG-specific evaluation — faithfulness, relevance, recall |
| [![Braintrust](https://img.shields.io/badge/Braintrust-F55036?style=flat-square)](https://www.braintrustdata.com) | Eval + logging + prompt management in one platform |
| [![OpenAI Evals](https://img.shields.io/badge/OpenAI_Evals-000000?style=flat-square&logo=openai&logoColor=white)](https://github.com/openai/evals) | Open-source eval framework from OpenAI |

<br/>

### Observability & Monitoring

Know what your model is doing in production.

| Tool | Type |
|------|------|
| [![Langfuse](https://img.shields.io/badge/Langfuse-000000?style=flat-square)](https://langfuse.com) | Open-source LLM tracing, analytics, and prompt management |
| [![LangSmith](https://img.shields.io/badge/LangSmith-1C3C3C?style=flat-square)](https://www.langsmith.com) | Tracing and debugging for LangChain apps |
| [![Helicone](https://img.shields.io/badge/Helicone-FF6B35?style=flat-square)](https://www.helicone.ai) | One-line proxy — logs every LLM call automatically |
| [![Arize AI](https://img.shields.io/badge/Arize_AI-0070F3?style=flat-square)](https://arize.com) | ML and LLM observability at enterprise scale |
| [![Opik](https://img.shields.io/badge/Opik-000000?style=flat-square)](https://www.comet.com/site/products/opik) | Open-source eval + observability from Comet |

<br/>

### Deployment & Serving

Getting models out of notebooks and into production.

| Tool | Best for |
|------|----------|
| [![Modal](https://img.shields.io/badge/Modal-000000?style=flat-square)](https://modal.com) | Serverless ML workloads — no infra management |
| [![Vercel AI SDK](https://img.shields.io/badge/Vercel_AI_SDK-000000?style=flat-square&logo=vercel)](https://sdk.vercel.ai) | Stream AI responses in web apps with minimal code |
| [![vLLM](https://img.shields.io/badge/vLLM-000000?style=flat-square)](https://github.com/vllm-project/vllm) | High-throughput inference engine for self-hosted models |
| [![BentoML](https://img.shields.io/badge/BentoML-000000?style=flat-square)](https://www.bentoml.com) | Package, serve, and scale ML models |
| [![Hugging Face Endpoints](https://img.shields.io/badge/HF_Endpoints-FFD21E?style=flat-square&logo=huggingface&logoColor=000)](https://huggingface.co/inference-endpoints) | One-click deployment for any HuggingFace model |
| [![Replicate](https://img.shields.io/badge/Replicate-000000?style=flat-square)](https://replicate.com) | Run any model via API — image, video, audio, text |

<br/>

### Dev Tooling

The local environment stack.

| Tool | What it is |
|------|------------|
| [![Claude Code](https://img.shields.io/badge/Claude_Code-000000?style=flat-square)](https://claude.ai/code) | Anthropic's agentic coding tool — runs in terminal, edits files |
| [![Cursor](https://img.shields.io/badge/Cursor-000000?style=flat-square)](https://www.cursor.com) | AI-native code editor — the IDE rebuilt around AI |
| [![Continue](https://img.shields.io/badge/Continue-000000?style=flat-square)](https://www.continue.dev) | Open-source AI code assistant for VS Code and JetBrains |
| [![Codeium](https://img.shields.io/badge/Codeium-09B37B?style=flat-square)](https://codeium.com) | Free AI autocomplete across 70+ languages |

---

## 🏗️ Founders & Builders

![Founders Banner](./assets/banner-founders.svg)

You're not deep in the infra — you're using AI to ship faster, validate ideas, and build real products. This section covers everything from prototyping to production-grade tooling without getting lost in the engineering.

<br/>

### Prototyping & Building Fast

| Tool | Why it matters |
|------|----------------|
| [![v0](https://img.shields.io/badge/v0_by_Vercel-000000?style=flat-square&logo=vercel)](https://v0.dev) | Text-to-UI — generate full React components from a prompt |
| [![Bolt](https://img.shields.io/badge/Bolt-000000?style=flat-square)](https://bolt.new) | Full-stack app builder in the browser — no local setup |
| [![Lovable](https://img.shields.io/badge/Lovable-FF6B35?style=flat-square)](https://lovable.dev) | AI-generated full-stack web apps with one-click deployment |
| [![Replit Agent](https://img.shields.io/badge/Replit-F26207?style=flat-square&logo=replit&logoColor=white)](https://replit.com/ai) | Build and deploy apps directly inside Replit |
| [![Cursor](https://img.shields.io/badge/Cursor-000000?style=flat-square)](https://www.cursor.com) | Fastest way to write production code with AI assistance |

<br/>

### AI-Powered Product Infrastructure

| Tool | What it gives you |
|------|------------------|
| [![OpenAI Platform](https://img.shields.io/badge/OpenAI_Platform-000000?style=flat-square&logo=openai&logoColor=white)](https://platform.openai.com) | Assistants API, function calling, file search — product-ready out of the box |
| [![Anthropic API](https://img.shields.io/badge/Anthropic_API-000000?style=flat-square)](https://console.anthropic.com) | Claude API — tool use, long documents, computer use |
| [![Vercel AI SDK](https://img.shields.io/badge/Vercel_AI_SDK-000000?style=flat-square&logo=vercel)](https://sdk.vercel.ai) | Streaming AI responses in any web framework |
| [![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)](https://supabase.com) | Postgres + pgvector + auth + storage — full backend for AI apps |

<br/>

### Voice & Multimodal

| Tool | Modality |
|------|----------|
| [![ElevenLabs](https://img.shields.io/badge/ElevenLabs-000000?style=flat-square)](https://elevenlabs.io) | Voice — best-in-class TTS, voice cloning, AI dubbing |
| [![AssemblyAI](https://img.shields.io/badge/AssemblyAI-000000?style=flat-square)](https://www.assemblyai.com) | Speech-to-text with built-in LLM features |
| [![Whisper](https://img.shields.io/badge/Whisper-000000?style=flat-square&logo=openai&logoColor=white)](https://github.com/openai/whisper) | Open-source STT — self-hostable, accurate, multilingual |
| [![Fal.ai](https://img.shields.io/badge/fal.ai-000000?style=flat-square)](https://fal.ai) | Fast inference for image and video generation |
| [![Runway](https://img.shields.io/badge/Runway-000000?style=flat-square)](https://runwayml.com) | AI video generation — Gen-3 Alpha |
| [![Sora](https://img.shields.io/badge/Sora-000000?style=flat-square&logo=openai&logoColor=white)](https://sora.com) | OpenAI's video generation model |

<br/>

### Cost, Routing & Optimization

| Tool | Purpose |
|------|---------|
| [![LiteLLM](https://img.shields.io/badge/LiteLLM-000000?style=flat-square)](https://litellm.ai) | Unified API across 100+ LLM providers — one interface, any model |
| [![OpenRouter](https://img.shields.io/badge/OpenRouter-000000?style=flat-square)](https://openrouter.ai) | Route to the cheapest or fastest model per request |
| [![Helicone](https://img.shields.io/badge/Helicone-FF6B35?style=flat-square)](https://www.helicone.ai) | Track spend, latency, and usage across providers |
| [![Portkey](https://img.shields.io/badge/Portkey-000000?style=flat-square)](https://portkey.ai) | AI gateway — load balancing, caching, fallbacks |

<br/>

### No-Code & Low-Code AI

| Tool | For |
|------|-----|
| [![Zapier AI](https://img.shields.io/badge/Zapier_AI-FF4A00?style=flat-square&logo=zapier&logoColor=white)](https://zapier.com/ai) | AI automation without writing code |
| [![Make](https://img.shields.io/badge/Make-6D00CC?style=flat-square)](https://make.com) | Visual workflow builder with AI module support |
| [![Flowise](https://img.shields.io/badge/Flowise-00C5A8?style=flat-square)](https://flowiseai.com) | Open-source drag-and-drop LLM app builder |
| [![Dify](https://img.shields.io/badge/Dify-000000?style=flat-square)](https://dify.ai) | Open-source LLMOps platform — no-code + API |

---

## 🔬 Researchers

![Researchers Banner](./assets/banner-researchers.svg)

You're working with models at a deeper level — training, evaluating, publishing. This section is for people pushing what's possible, not just consuming what exists.

<br/>

### Open Models & Weights

| Model | Released by | Why it matters |
|-------|-------------|----------------|
| [![Llama 3](https://img.shields.io/badge/Llama_3-0064e0?style=flat-square&logo=meta&logoColor=white)](https://llama.meta.com) | Meta | Most widely adopted open model family |
| [![Mistral / Mixtral](https://img.shields.io/badge/Mistral-000000?style=flat-square)](https://mistral.ai/models) | Mistral AI | MoE architecture — high performance, efficient |
| [![Qwen 2.5](https://img.shields.io/badge/Qwen_2.5-FF6A00?style=flat-square)](https://qwenlm.github.io) | Alibaba | Multilingual, strong coding and math |
| [![Gemma 3](https://img.shields.io/badge/Gemma_3-4285F4?style=flat-square&logo=google&logoColor=white)](https://ai.google.dev/gemma) | Google | Lightweight, optimized for research and edge |
| [![DeepSeek R1](https://img.shields.io/badge/DeepSeek_R1-000000?style=flat-square)](https://deepseek.com) | DeepSeek | Open reasoning model — competitive with o1 |
| [![Phi-4](https://img.shields.io/badge/Phi--4-512BD4?style=flat-square&logo=microsoft)](https://huggingface.co/microsoft/phi-4) | Microsoft | Small model, surprisingly capable |

<br/>

### Platforms for Open Models

| Tool | What it provides |
|------|-----------------|
| [![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=000)](https://huggingface.co) | The central hub — models, datasets, spaces, inference |
| [![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square)](https://ollama.com) | Run any open model locally with one command |
| [![Together AI](https://img.shields.io/badge/Together_AI-000000?style=flat-square)](https://www.together.ai) | Fine-tune and run open models on shared GPU infra |
| [![Replicate](https://img.shields.io/badge/Replicate-000000?style=flat-square)](https://replicate.com) | Version and run models with a versioned API |

<br/>

### Fine-tuning

| Tool | Best for |
|------|----------|
| [![Unsloth](https://img.shields.io/badge/Unsloth-000000?style=flat-square)](https://github.com/unslothai/unsloth) | 2x faster fine-tuning, 70% less VRAM — use this first |
| [![Axolotl](https://img.shields.io/badge/Axolotl-000000?style=flat-square)](https://github.com/axolotl-ai-cloud/axolotl) | Streamlined fine-tuning with broad architecture support |
| [![LLaMA-Factory](https://img.shields.io/badge/LLaMA--Factory-000000?style=flat-square)](https://github.com/hiyouga/LLaMA-Factory) | Fine-tune 100+ models in one unified framework |
| [![OpenAI Fine-tuning](https://img.shields.io/badge/OpenAI_Fine--tuning-000000?style=flat-square&logo=openai&logoColor=white)](https://platform.openai.com/docs/guides/fine-tuning) | Managed fine-tuning for GPT models |
| [![Fireworks Fine-tuning](https://img.shields.io/badge/Fireworks_Fine--tuning-FF6B35?style=flat-square)](https://fireworks.ai/fine-tuning) | Cloud fine-tuning with fast inference on completion |

<br/>

### Benchmarks & Evaluation Frameworks

| Benchmark | Tests |
|-----------|-------|
| [MMLU](https://github.com/hendrycks/test) | Massive multitask language understanding across 57 subjects |
| [HumanEval](https://github.com/openai/human-eval) | Code generation — OpenAI's standard coding benchmark |
| [HELM](https://crfm.stanford.edu/helm) | Holistic evaluation across accuracy, fairness, robustness |
| [BIG-Bench Hard](https://github.com/suzgunmirac/BIG-Bench-Hard) | Challenging tasks that stump current models |
| [LMSYS Chatbot Arena](https://chat.lmsys.org) | Human preference ranking — the most credible leaderboard |
| [LiveBench](https://livebench.ai) | Contamination-free benchmark updated monthly |

<br/>

### Essential Reading

| Resource | What it covers |
|----------|----------------|
| [Attention Is All You Need](https://arxiv.org/abs/1706.03762) | The transformer paper — where modern AI begins |
| [Scaling Laws for Neural LMs](https://arxiv.org/abs/2001.08361) | How compute, data, and model size interact |
| [Constitutional AI](https://arxiv.org/abs/2212.08073) | Anthropic's RLHF alternative — the basis for Claude |
| [RLHF Survey](https://arxiv.org/abs/2307.01928) | Comprehensive overview of reinforcement learning from human feedback |
| [RAG Paper](https://arxiv.org/abs/2005.11401) | The original retrieval-augmented generation paper |
| [Chain-of-Thought Prompting](https://arxiv.org/abs/2201.11903) | Why reasoning steps improve outputs |
| [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer) | Best visual explanation of how transformers work |
| [Anthropic Interpretability Research](https://www.anthropic.com/research) | What's actually inside these models |

---

## Contributing

This is a living reference. If something belongs here, open a PR.

**Standards for inclusion:**
- The tool must be actively maintained
- It must serve a real function in the stack — not just hype
- One sentence must be enough to explain what it does

**If you're adding a tool**, use the existing table format and place it in the right layer.

---

<div align="center">

<br/>

*Maintained by* &nbsp;
[![𝕏 @chitajohn_](https://img.shields.io/badge/@chitajohn__-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/chitajohn_)

<br/>

[MIT License](LICENSE) &nbsp;·&nbsp; Star if this helped &nbsp;·&nbsp; Share if it belongs in someone's stack

<br/>

</div>
