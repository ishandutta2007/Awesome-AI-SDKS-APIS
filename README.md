# Awesome-AI-SDKS-APIS
# Awesome-AI-SDKS-APIS

## Top AI SDKs & APIs Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Provider SDKs, Multi-Model Gateways & Agent Orchestration Frameworks*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI SDKs & APIs**. These tools enable developers to integrate language models into applications—from official provider SDKs with native tracing to unified multi-provider abstractions that reduce vendor lock-in.



**Examples** include OpenAI SDK, Anthropic SDK, Google Gen AI SDK, AWS Bedrock SDK, Cohere SDK, Mistral SDK, LangChain, LlamaIndex, LiteLLM, and Vercel AI SDK (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, multi-provider abstraction, and open agent infrastructure—ideal for developers, platform teams, and organizations seeking transparent, vendor-independent AI integration.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global AI API market is estimated at approximately $44B–$65B in 2025 and projected to reach $83B–$85B by 2026, driven by a ~30–32% CAGR as enterprise generative AI workloads transition from experimental development to production-scale inference and agentic automation. The sector is moderately concentrated among an oligopoly of mega-cap hyperscalers (Microsoft, Alphabet, Amazon) and frontier lab providers (OpenAI, Anthropic) capturing the vast majority of enterprise inference volume, while remaining fragmented across open-weight specialized providers and multi-model gateway architectures.

## SaaS/Hosted Platforms

| Company / Product | Description & Capabilities | Company Size (Valuation / Revenue) | Starting Tier Pricing | Free Tier / Trial Limits |
| :--- | :--- | :--- | :--- | :--- |
| **[Azure OpenAI Service](https://azure.microsoft.com/en-us/products/ai-services/openai-service)** | Microsoft's enterprise-managed OpenAI models with security, enterprise compliance, virtual networks, and regional data residency. Accessible via REST APIs and the OpenAI SDK. | **Microsoft**: ~$3.1T Market Cap / $245B+ Annual Revenue | **$0.150 / 1M input tokens** & **$0.600 / 1M output tokens** (GPT-4o-mini standard pay-as-you-go) | **$200 credit** (valid 30 days on Azure Free Trial; requires upgrading subscription to Pay-As-You-Go with $0 spend to unlock 0 TPM default LLM quota limits) |
| **[AWS Bedrock](https://aws.amazon.com/bedrock/)** | Fully managed foundation model service offering Anthropic Claude, Amazon Nova/Titan, Meta Llama, Mistral, and Cohere with automated guardrails, RAG knowledge bases, and multi-agent routing. | **Amazon**: ~$2.2T Market Cap / $620B+ Annual Revenue | **$0.06 / 1M input tokens** & **$0.24 / 1M output tokens** (Amazon Nova Micro on-demand) | **$100–$200 AWS Promotional Credits** (valid 30 days to 6 months upon account activation/onboarding prompt tasks; no perpetual free tier) |
| **[Google Gemini API](https://ai.google.dev/)** | Official API for Gemini models via Google AI Studio and Vertex AI. Supported by the unified `google-genai` SDK and Google Agent Development Kit (ADK) across Python, JS/TS, Go, and Java. | **Alphabet**: ~$2.1T Market Cap / $350B+ Annual Revenue | **$0.075 / 1M input tokens** & **$0.30 / 1M output tokens** (Gemini 2.5 Flash / 1.5 Flash paid tier up to 128k prompt context) | **Free Forever Tier**: 15 RPM (requests/min), 1,000,000 TPM (tokens/min), and 1,500 RPD (requests/day) on Gemini Flash models in Google AI Studio |
| **[OpenAI API](https://platform.openai.com/)** | Industry-standard API powering GPT-4o, GPT-4o-mini, o-series reasoning models, DALL-E, Whisper, and Embeddings. Supported by OpenAI Agents SDK with native MCP and guardrails. | **OpenAI**: ~$157B Valuation (Oct 2024 funding round) / ~$3.7B–$5B Annualized Revenue | **$0.150 / 1M input tokens** & **$0.600 / 1M output tokens** (GPT-4o-mini pay-as-you-go; minimum $5 initial balance deposit) | **Pay-as-you-go only (0 automatic free signup credits)**; requires $5 minimum deposit (Free testing tier available via Researcher Grants up to $1,000 or opt-in training data sharing allocations) |
| **[Anthropic API](https://www.anthropic.com/api)** | Official API for Claude 3.5/3.7 models (Haiku, Sonnet, Opus). Powers the Claude Agent SDK with built-in sub-agent tools, tool call interception hooks, and first-class Model Context Protocol (MCP) support. | **Anthropic**: ~$60B Valuation (early 2025 / late 2024 funding) / ~$1B+ Annualized Revenue | **$0.80 / 1M input tokens** & **$4.00 / 1M output tokens** (Claude 3.5 Haiku pay-as-you-go) | **$5 one-time free credit** upon phone verification in Anthropic Console (expires upon balance depletion; no perpetual free tier) |
| **[Mistral AI Platform](https://mistral.ai/)** | Official API (La Plateforme) for European frontier open-weight models including Mistral Large, Mistral Small, Codestral, and Pixtral with Apache-2.0 or commercial license endpoints. | **Mistral AI**: ~$6.2B Valuation / ~$30M+ Annualized Revenue | **$0.10 / 1M input tokens** & **$0.30 / 1M output tokens** (Mistral Small / Codestral serverless pay-as-you-go) | **Free Mode (Experimental Tier)**: Free API access with no credit card required, rate-limited to 1 RPS (request/sec) for personal experimentation and prototyping |
| **[Cohere Platform](https://cohere.com/)** | Enterprise-focused API platform for Command R+, Command R, Embed v3, and Rerank v3 models. Supports private cloud, on-premises, and VPC enterprise deployments. | **Cohere**: ~$5.5B Valuation / ~$35M+ Annualized Revenue | **$0.15 / 1M input tokens** & **$0.60 / 1M output tokens** (Command R fine-tuned/production pay-as-you-go; Embed from $0.10 / 1M tokens) | **Free Trial Key (Free Forever for Dev)**: Up to 1,000 API calls per month, rate-limited to 20 RPM (Chat) and 5 RPM (Embed) for non-commercial prototyping |



## Open-Source GitHub Projects



- **[OpenAI SDK (openai-python)](https://github.com/openai/openai-python)**  

  **The official Python library for the OpenAI API** (Apache-2.0) . The reference implementation for API client design—provides convenient access to the OpenAI API from Python applications . **The most widely used AI SDK in the ecosystem.** **Bundle size: 34.3 kB gzipped** (smallest, most efficient for client-side) .



- **[OpenAI SDK (openai-node)](https://github.com/openai/openai-node)**  

  **The official JavaScript/TypeScript library for the OpenAI API** (Apache-2.0) . Generated from the same OpenAPI specification as the Python SDK, ensuring API parity across languages.



- **[Anthropic SDK (anthropic-sdk-python)](https://github.com/anthropics/anthropic-sdk-python)**  

  **The official Python library for the Anthropic API** (MIT) . Provides access to Claude models with `client.messages.create()` interface . **v1.14.0** (October 2026) adds **native OpenTelemetry tracing support**—spans created with global tracer provider, exported with existing traces, and trace context headers propagated from the global propagator . **Python 3.9+** required .



- **[Google Gen AI SDK (googleapis/python-genai)](https://github.com/googleapis/python-genai)**  

  **The official Python SDK for the Gemini API** (Apache-2.0) . **GA since May 2025** and the recommended library for all Gemini API access . Install via `pip install google-genai` . **Replaces the legacy `google-generativeai` library**, which is no longer maintained and was deprecated November 30, 2025 . Available for Python, JavaScript/TypeScript, Go, and Java .



- **[Vercel AI SDK](https://github.com/vercel/ai)**  

  **The AI Toolkit for TypeScript** (Apache-2.0) from the creators of Next.js . **Unified interface for multiple AI providers**—OpenAI, Anthropic, Google, Azure, Amazon Bedrock, and more . Core APIs: `generateText`, `streamText`, `generateObject`, `streamObject`, `embed`/`embedMany`, `generateImage`, `tool`, `jsonSchema`/`zodSchema` . **The standard for building AI applications in Next.js and React.** **Bundle size: 67.5 kB gzipped** (2x OpenAI, acceptable for modern web apps) . **Edge-compatible** with native V8 support .



- **[LlamaIndex](https://github.com/run-llama/llama_index)**  

  **The leading specialized data framework for building production RAG systems** (MIT) . **40,000+ GitHub stars**, founded by Jerry Liu in late 2022 . Provides **500+ data connectors** (LlamaHub), advanced indexing strategies (vector, keyword, knowledge graph), and sophisticated retrieval pipelines with reranking, query transformation, and response synthesis . Available in Python and TypeScript . **LlamaParse** handles complex PDFs and tables better than most alternatives . **Note**: API has evolved rapidly with significant breaking changes between versions; agent capabilities are less mature than dedicated frameworks like CrewAI or LangGraph .



- **[LiteLLM](https://github.com/BerriAI/litellm)**  

  **The fastest, litest AI Gateway** (MIT) — **Rust core with Python SDK** . **Call 100+ LLM APIs in OpenAI format**—Bedrock, Azure, OpenAI, Anthropic, VertexAI, vLLM, Nvidia NIM, Cohere, and more . Features **cost tracking, guardrails, load balancing, and logging** . Docker images signed with **cosign** for supply chain security . **The de facto standard for multi-provider orchestration**—powers many other aggregators including LibreChat, Open WebUI, and Dify . **P99 latency: 0.66ms** (own benchmark) .



- **[LangChain](https://github.com/langchain-ai/langchain)**  

  **The most widely adopted framework for building LLM applications** (MIT) . **`create_agent` provides a minimal, highly configurable agent harness**—compose exactly the agent your use case needs from model, tools, prompt, and middleware . Supports OpenAI, Anthropic, Google, OpenRouter, Fireworks, Baseten, and Ollama . **The de facto standard for LLM application development.** **Bundle size: 101.2 kB gzipped** (3x OpenAI, reflects comprehensive features) . **LangGraph** (v1.0.10) provides graph-based state machines with persistent checkpointing, crash recovery, and time-travel debugging .



- **[Haystack (deepset)](https://github.com/deepset-ai/haystack)**  

  **Production-ready NLP framework** (Apache-2.0). Features **typed pipelines** for RAG, question answering, and semantic search . **Strong enterprise focus** with component-based architecture and extensive evaluation tools . **Recommended for production-grade typed RAG pipelines** .



### Additional Strong Open-Source Options



- **[OpenAI OpenAPI Specification](https://github.com/openai/openai-openapi)** — The **source of truth for OpenAI API SDKs** . Generated SDKs in Python and JavaScript/TypeScript.

- **[Anthropic SDK (anthropic-sdk-typescript)](https://github.com/anthropics/anthropic-sdk-typescript)** — Official TypeScript SDK for Claude API (MIT).

- **[Google Gen AI SDK (googleapis/js-genai)](https://github.com/googleapis/js-genai)** — Official TypeScript SDK for Gemini API .

- **[AWS SDK for Python (boto3)](https://github.com/boto/boto3)** — Official AWS SDK including Bedrock client (Apache-2.0).

- **[Cohere Python SDK](https://github.com/cohere-ai/cohere-python)** — Official Python SDK for Cohere API.

- **[Mistral Python Client](https://github.com/mistralai/client-python)** — Official Python SDK for Mistral API.

- **[Portkey Gateway](https://github.com/Portkey-AI/gateway)** — Blazing fast AI gateway with 250+ models and 45+ guardrails (Apache-2.0 core). Features routing strategies, caching, retries, and observability. Semantic caching and guardrails run on Portkey's infrastructure when using the managed tier .

- **[RouteLLM](https://github.com/lm-sys/RouteLLM)** — Open-source routing framework (Apache-2.0) that decides which model should handle a request. Achieves roughly **95% of GPT-4-level quality at 14% of the strong-model call volume** on LMSYS benchmarks .

- Community **n8n** workflows for AI SDK integration testing and multi-provider orchestration.



**Frameworks for building custom systems**: Combine **LiteLLM** for multi-provider gateway orchestration with **Vercel AI SDK** for TypeScript application development, **LlamaIndex** for RAG pipelines, **Anthropic SDK** or **OpenAI SDK** for direct provider access, and **Haystack** for production typed RAG—creating a comprehensive AI SDK stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AI SDKs and APIs handling prompts and API keys must comply with data protection regulations (GDPR, CCPA, etc.) and provider terms of service.

- **Official SDKs are the reference implementation.** OpenAI's SDKs are generated from the published **OpenAPI specification** . Anthropic's Python SDK adds **native OpenTelemetry tracing** . Google's **GenAI SDK is GA** and replaces the deprecated legacy libraries . **These are maintained by the model providers and are the recommended integration path.**

- **Multi-provider abstraction reduces lock-in.** Vercel AI SDK provides a **unified interface across 25+ providers** . LiteLLM calls **100+ LLM APIs in OpenAI format** with cost tracking and guardrails . **These are the pragmatic choice when you need provider flexibility.**

- **RAG frameworks are specialized, not general-purpose.** LlamaIndex is **data-first** with 500+ connectors and advanced retrieval pipelines . Haystack offers **typed pipelines** for production RAG . **Choose based on your primary use case, not popularity alone.**

- **Edge deployment creates critical constraints.** Vercel AI SDK offers **explicit edge support with native V8 compatibility**. LangChain JS is **fundamentally incompatible** due to Node.js `fs` module usage. OpenAI SDK requires the `openai-edge` variant . **If your architecture requires edge deployment, LangChain JS cannot be used regardless of other factors.**

- Self-hosted open-source solutions require proper security hardening, API key management, and ongoing maintenance. **SDK version pinning is essential**—breaking changes between versions are common, especially in rapidly evolving frameworks like LlamaIndex .



---



**Made for developers, platform teams, and organizations building transparent AI integration solutions.**  

Let's make AI SDKs & APIs more open, data-driven, and provider-independent.
