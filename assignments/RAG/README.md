# RAG with Chunking, Vector Database (FAISS) and Source Citations

This project implements a **Retrieval-Augmented Generation (RAG)** system that answers user questions using a collection of documents. The system retrieves relevant information from documents using **vector similarity search** and generates answers using a **Large Language Model (LLM)**.

## Overview

This project builds a RAG pipeline that:

1. Splits documents into smaller chunks.
2. Converts each chunk into embeddings (vectors).
3. Stores the embeddings in a **vector database**.
4. Retrieves the most relevant chunks for a user query.
5. Generates an answer using the retrieved context.
6. Displays the **source documents used for the answer**.


## Why Chunking is Important

Instead of embedding an entire article as a single vector, documents are split into smaller **chunks**. This improves retrieval accuracy because the system can retrieve the **specific part of a document that contains the answer** rather than returning the whole article.


## Why Use a Vector Database

A **vector database** stores embeddings and enables efficient similarity search.

Using a vector database provides several advantages:

* **Fast similarity search** across large numbers of embeddings.
* **Scalability** to millions of documents.
* Efficient **nearest neighbor retrieval** for semantic search.
* Better performance compared to manually computing similarity across all embeddings.

In this project we use **FAISS**, a high-performance vector search library designed for efficient similarity search over large embedding collections.

## Technologies Used

* **Python**
* **Pandas** – Data processing
* **NumPy** – Vector operations
* **Sentence Transformers** – Text embeddings
* **FAISS** – Vector database for similarity search
* **Google Gemini API** – LLM for answer generation
* **tqdm** – Progress tracking

## Requirements

Install the required libraries:

```
pip install sentence-transformers pandas numpy google-genai tqdm faiss-cpu
```

## How to run

1. Place the dataset containing the articles in the project directory.
2. Run the notebook.
3. Enter a query.
4. The system retrieves relevant chunks and generates an answer with source citations.


