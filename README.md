# Retrieval-Augmented Generation (RAG) System with ChromaDB and LangChain

This repository implements a Retrieval-Augmented Generation (RAG) system that allows you to query a private document and receive answers based on the document's content.  It leverages ChromaDB for vector storage and retrieval, LangChain for orchestrating the RAG pipeline, and a free, open-source LLM for generating responses.

## Overview

This project creates a bot that can answer questions based on a private document (TXT, PDF, or other text-based files).  The document is processed, chunked, and embedded into a vector database using ChromaDB. When a user asks a question, the system retrieves relevant chunks from the database, uses them as context in a prompt, and sends the prompt to an LLM. The LLM generates an answer based on the provided context.

## Features

* **Document Ingestion:**  Processes text-based documents (TXT, PDF, etc.) for indexing.
* **Vector Database:** Uses ChromaDB to store and retrieve document embeddings.
* **Contextual Retrieval:**  Retrieves relevant document chunks based on user queries.
* **LLM Integration:**  Uses microsoft/Phi-3-mini-4k-instruct
* **LangChain Orchestration:** Employs LangChain to manage the retrieval and LLM interaction.

## Getting Started

### Prerequisites

* Python 3.11.x
* All dependencies listed in requirements.txt. Use:
```bash
pip install -r .\requirements.txt


