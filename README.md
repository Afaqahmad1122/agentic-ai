# Agentic AI Crash Course

Hands-on notebooks covering LLM calls, RAG, vector databases, and agents with LangChain, Google Gemini, and Groq.

## Contents

- 1_simple_llm_calling: basic LLM calls
- 2_health_analysis: blood work analysis with an LLM
- 3_vector_db: vector database basics with Chroma
- rag_basics: retrieval augmented generation over a PDF
- single_agent: a single tool-using agent
- product_query_agent: a product query agent

## Setup

Requires Python 3.14+ and [uv](https://docs.astral.sh/uv/).

```
uv sync
```

Create a `.env` file in the project root:

```
GOOGLE_API_KEY=your_key
GROQ_API_KEY=your_key
```

## Run

```
uv run jupyter notebook
```
