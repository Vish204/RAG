# Semantic Document Search (RAG Retrieval Component)

This project implements a **semantic document search engine** using vector embeddings and similarity search.  
It forms the **retrieval module** of a Retrieval-Augmented Generation (RAG) pipeline.

The system extracts text from PDF documents, converts text chunks into embeddings using a transformer model, and retrieves the most semantically relevant paragraphs for a user query using vector similarity.

---

## Project Overview

Traditional keyword-based search fails to capture meaning.  
This project uses **semantic embeddings** to retrieve contextually relevant document sections.

Pipeline:

PDF Documents → Text Extraction → Chunking → Embeddings → FAISS Vector Index → Query Search

This retrieval output can later be passed to a Large Language Model (LLM) to complete a full RAG system.

---

## Features

- PDF text extraction using PyMuPDF  
- Paragraph-level text chunking  
- Semantic embeddings using Sentence Transformers  
- Fast vector similarity search using FAISS  
- Top-k paragraph retrieval for user queries  

---

## Technologies Used

- Python  
- Sentence Transformers  
- FAISS  
- NumPy  
- PyMuPDF  
- Google Colab

---

## Architecture

1. Load PDF documents  
2. Extract text from each page  
3. Split text into paragraphs (chunking)  
4. Convert paragraphs into embeddings  
5. Store embeddings in FAISS vector index  
6. Convert user query into embedding  
7. Retrieve top-k similar paragraphs  

---

## Installation

Clone the repository:
git clone https://github.com/<your-username>/RAG.git
cd RAG

## Install dependencies:
pip install sentence-transformers faiss-cpu pymupdf numpy
