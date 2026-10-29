# CoreIndex: Vectorless, Reasoning-based RAG

**Reasoning-based RAG ◦ No Vector DB, No Chunking ◦ Context-Aware Retrieval ◦ Reads Like a Human**

#### [🌐 Website](#) • [☁️ Cloud](#) • [📖 Docs](#) • [📝 Blog](#) • [✉️ Contact](#)

---


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
