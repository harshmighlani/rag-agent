# rag-agent

This project implements a complete Retrieval-Augmented Generation (RAG) system using:

ChromaDB (SQLite backend) for vector storage

BAAI/bge-small-en-v1.5 for high-performance, free sentence embeddings

Groq LLaMA-3.1 (8B Instant) for fast, accurate responses

LangChain (community components) for loaders, chunking, and retrieval

The agent loads local PDFs, chunks them, embeds the chunks, stores them into ChromaDB, and answers user questions using retrieval + LLM.

🚀 Features

✅ Load all PDFs from the current directory 

✅ Chunk documents using LangChain’s recursive splitter

✅ Generate 1024-dim embeddings using BAAI

✅ Store vectors in a local ChromaDB SQLite database

✅ Retrieve relevant chunks using similarity search

✅ Answer questions via Groq’s LLaMA-3.1 model

✅ Fully interactive question→answer agent loop

📂 Project Structure
project/
│── rag_agent.py           # Main RAG pipeline script

│── .env                   # Contains GROQ_API_KEY

│── sample.pdf             # Your documents (any PDFs placed here are loaded)

│── rag_sqlite_db/         # ChromaDB SQLite vector store (created on first run)

🧩 Requirements

Python 3.10+ (tested on Python 3.13)

A Groq API Key → https://console.groq.com/keys
