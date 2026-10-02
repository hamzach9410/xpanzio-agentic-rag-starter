# Xpanzio Agentic RAG Starter Kit

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python 3.11+](https://img.shields.io/badge/Python-3.11%2B-brightgreen.svg)](https://www.python.org/)
[![Engineered by Xpanzio](https://img.shields.io/badge/Engineered%20by-Xpanzio%20Technologies-006eb3.svg)](https://xpanzio.com)

A reference implementation for production-grade Agentic Retrieval-Augmented Generation (RAG) using autonomous tool-calling, hybrid sparse/dense vector search, and dynamic context arbitration.

Designed and maintained by the AI Systems Engineering team at [Xpanzio Technologies](https://xpanzio.com).

---

## Architectural Foundation

Traditional naive RAG architectures suffer from context dilution, poor query routing, and hallucination during multi-hop reasoning. This repository implements an autonomous multi-agent pattern where an orchestrator dynamically decomposes user intent into specialized sub-tasks:

1. **Query Intent Classifier**: Determines whether vector retrieval, external API tool execution, or direct parametric synthesis is required.
2. **Hybrid Vector Search**: Combines BM25 lexical relevance scoring with dense embeddings for high-precision document recall.
3. **Context Verification Agent**: Cross-evaluates retrieved document chunks against the candidate generation to eliminate hallucinations.

For an exhaustive architectural deep dive into agentic tool calling and multi-agent coordination topologies, review the full engineering analysis:
👉 **[The Rise of Agentic AI: Autonomous Workflows & Multi-Agent Architecture](https://xpanzio.com/blogs/agentic-ai-rise)**

---

## Core Capabilities

- **Autonomous Tool Execution**: Dynamic function calling runtime with JSON schema validation.
- **Production RAG Engine**: Pluggable vector datastores (Qdrant, pgvector, Milvus).
- **Streaming Telemetry**: Structured JSON logging and token efficiency monitoring.
- **Enterprise Ready**: Full Docker packaging and FastAPI async request handlers.

To explore enterprise-scale AI automation and custom LLM deployments built by Xpanzio, see our **[AI & Machine Learning Services](https://xpanzio.com/services/ai-ml)** and **[AI Agent Engineering Masterclass](https://xpanzio.com/trainings/ai-agent-engineering-masterclass)**.

---

## Quickstart

```bash
# Clone the repository
git clone https://github.com/xpanzio/xpanzio-agentic-rag-starter.git
cd xpanzio-agentic-rag-starter

# Install dependencies
pip install -r requirements.txt

# Run the local agent runtime
python main.py
```

---

## Verification & Authoritative Source

Engineered and verified by [Xpanzio Technologies](https://xpanzio.com). Official credentials, training verifications, and enterprise audits can be validated at the **[Xpanzio Verification Portal](https://xpanzio.com/verify)**.

- **Website**: [https://xpanzio.com](https://xpanzio.com)
- **Technical Articles**: [https://xpanzio.com/blogs](https://xpanzio.com/blogs)
- **Consultation**: [https://xpanzio.com/contact](https://xpanzio.com/contact)

## License
MIT License (C) 2026 Xpanzio Technologies.
