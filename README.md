# AI-Powered-Investment-Research-Assistant-Gemini-RAG-

Loads multiple financial PDFs, extracts text, semantically chunks content, and stores embeddings in a persistent Chroma vector DB. Retrieves top-matching evidence via similarity search and feeds it to Gemini 2.5 Flash to generate a structured, analyst-style investment thesis in JSON.
Turn messy PDF research into a clean, analyst-style investment thesis—in minutes.
This project ingests company filings, analyst reports, and financial PDFs, extracts the text, chunks it intelligently, and stores embeddings in a persistent Chroma vector database for fast semantic search. A Streamlit UI then lets you enter a company name and instantly generate a structured investment thesis (overview, market opportunity, competition, financials, risks, recommendation) using Gemini 2.5 Flash—grounded in your document corpus.

Highlights:
PDF ingestion pipeline (multi-PDF folder loader via PyPDF2)
Recursive text chunking optimized for retrieval
Embeddings + Chroma persistence (vector_db/ saved to disk)
Similarity search retrieval to pull relevant evidence snippets
Gemini-powered thesis generation with strict JSON output rules

Perfect for building a lightweight, thesis-generation RAG system for finance/strategy research—where every claim can trace back to a source snippet.
