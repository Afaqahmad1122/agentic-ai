# Agentic AI Crash Course

Hands-on notebooks covering LLM calls, RAG, vector databases, and agents with LangChain, Google Gemini, and Groq.

## Contents

- 1_simple_llm_calling/call_llm.ipynb: calls Gemini through LangChain with a plain prompt, a system plus human message list, and different temperature values (0 vs 1).
- 2_health_analysis/blood_work.ipynb: reads a sample report (blood_work.txt) and prompts Gemini to extract every test value and label it HIGH, LOW or NORMAL against the reference ranges. This is stage 1 of a multi-stage analysis.
- 3_vector_db/vectordb_basics.ipynb: stores four short news snippets in an in-memory Chroma collection and prints the embeddings it generates for each one.
- rag_basics/rag.ipynb: full RAG pipeline over telecom_guide.pdf. It loads the PDF, splits it into 600 character chunks, embeds them with all-MiniLM-L6-v2 into Chroma, retrieves the top 3 chunks, and answers using only that context with Gemini.
- single_agent/single_agent.ipynb: placeholder notebook, currently empty.
- product_query_agent/product_auery_agent.ipynb: a LangChain agent (Groq model) with a get_product tool that looks up price and description from an in-memory product catalog.

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
