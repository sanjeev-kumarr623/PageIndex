# CoreIndex: Vectorless, Reasoning-based RAG

**Reasoning-based RAG ◦ No Vector DB, No Chunking ◦ Context-Aware Retrieval ◦ Reads Like a Human**

#### [🌐 Website](#) • [☁️ Cloud](#) • [📖 Docs](#) • [📝 Blog](#) • [✉️ Contact](#)

---

<details open>
<summary><h2>Updates</h2></summary>

- [Oct '26] 🔥 [**Page Search API**](#): find the pages that answer each question in about a second, and send your LLM only those. *Cut 97% token cost on document question answering*; more accurate and faster than vector search.
- [Aug '26] [**SDK**](#quickstart): **local** and **cloud** modes — one client to index, retrieve, and chat on your machine (with your own LLM API key) or on Cloud.
- [Aug '26] ⚡ [**Flash Indexing**](#): fast tree index generation for text-based PDFs, now the default indexing method in SDK local mode.
- [Scale to Millions of Documents](#): *File System* is a file-level tree indexing layer that lets the engine reason over an entire corpus, not just a single document.
- [App Experience](#): a human-like document analysis agent for long professional documents.

</details>

---

# What is CoreIndex?

Are you frustrated with vector database retrieval accuracy for long and complex documents? Vector-based RAG retrieves by semantic **similarity**. But **similarity ≠ relevance** — what retrieval actually needs is relevance, and relevance requires **reasoning**. On professional documents that demand contextual understanding, domain expertise, and multi-step reasoning, similarity search misses what is relevant but not similar, and returns what is similar but not relevant.

Inspired by advanced tree-search paradigms, **CoreIndex** replaces the vector index with a **hierarchical tree index** and lets an LLM **reason** its way through it, the way a human expert turns to and reads the right section of a long report. Retrieval happens in two steps:

1. **Index**: generate a **tree-structure index** for each document
2. **Retrieve**: agentically **search that tree** with LLM reasoning

### TL;DR

> CoreIndex is a **vectorless**, **reasoning-based RAG** engine that **mirrors how humans read**, delivering **traceable**, **explainable**, and **context-aware** retrieval, with **no vector DBs** or **chunking**.

### Compare with Vector RAG

| | Vector RAG | **CoreIndex** |
|---|---|---|
| **Index** | vector index | tree index |
| **Retrieval** | semantic similarity search | LLM reasoning over the tree |
| **Result** | opaque, “vibe retrieval” | traceable to explicit references |
| **Context** | query embedding only | full context: conversation history, domain knowledge, etc. |

It is ideal for financial reports, legal documents, regulatory filings, technical manuals, medical literature, academic textbooks, and any other long, complex professional document.

---

# Quickstart

```bash
pip install -U core-index
