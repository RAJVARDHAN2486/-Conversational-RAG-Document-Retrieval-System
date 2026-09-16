
# Retrieval-Augmented Generation (RAG) From Scratch


The project focuses on understanding how RAG works internally rather than relying entirely on high-level frameworks. It covers the complete pipeline from document ingestion and chunking to embeddings, vector search, context augmentation, and LLM generation.

## RAG Pipeline

```text
Documents
   ↓
Document Loader
   ↓
Text Chunking
   ↓
Embedding Generation
   ↓
Vector Database
   ↓
Query Embedding
   ↓
Similarity Search / Retrieval
   ↓
Context Augmentation
   ↓
LLM Generation
   ↓
Answer
```

## What This Project Covers

### Core RAG

* Introduction to RAG and its architecture
* Vector embeddings
* Document/data ingestion
* Text chunking and splitting
* Document retrieval
* Cosine similarity
* Building a RAG pipeline from scratch
* Conversational RAG with chat history

### Advanced RAG Techniques

* Recursive text splitting
* Semantic chunking
* Advanced document chunking
* Advanced retrieval techniques
* Multi-query RAG
* Reciprocal Rank Fusion (RRF)
* Hybrid search using vector and keyword search
* RAG reranking
* Multimodal RAG with images and documents
* Agent-based document chunking

## Implementation Approach

The core concepts are implemented with simple Python code so that each part of the RAG pipeline can be understood independently.

For example:

```python
Document → Chunks → Embeddings → Vector Store
Query → Embedding → Retrieval → Context → LLM → Answer
```

The project also demonstrates concepts such as storing document chunks alongside their embeddings and using similarity search to retrieve the most relevant chunks.

## Key Concepts

### Embeddings

Convert text into numerical vectors that represent semantic meaning.

### Vector Search

Compare the query embedding with document embeddings to find semantically similar content.

### Chunking

Split large documents into smaller pieces so that relevant information can be retrieved efficiently.

### Retrieval

Select the most relevant chunks from the stored documents based on similarity.

### Augmentation

Combine the retrieved context with the user's query to construct a prompt for the language model.

### Generation

Pass the augmented prompt to an LLM to generate the final answer.

## Learning Goals

This repository is intended to build a strong understanding of:

* How RAG works internally
* Why embeddings are needed
* How vector similarity search works
* How chunking affects retrieval quality
* How retrieved context is passed to an LLM
* How advanced retrieval strategies improve RAG systems

## Tech Stack

* Python
* Embedding Models
* Vector Search
* Large Language Models (LLMs)
* RAG techniques
* HTTP APIs

## Project Structure

```text
rag-from-scratch/
│
├── data/              # Source documents
├── embeddings/        # Embedding-related code
├── retrieval/         # Vector search and retrieval
├── chunking/          # Text splitting strategies
├── generation/        # LLM generation
├── examples/          # RAG examples
├── requirements.txt
└── README.md
```

## Why From Scratch?

The goal is to understand the **fundamentals behind RAG**, rather than treating a framework as a black box.

This makes it easier to understand what libraries such as LangChain and vector databases are doing internally and provides a stronger foundation for designing and debugging production RAG systems.

## Topics Covered

```text
RAG Architecture
     ↓
Embeddings
     ↓
Data Ingestion
     ↓
Chunking
     ↓
Vector Search
     ↓
Cosine Similarity
     ↓
Retrieval
     ↓
Prompt Augmentation
     ↓
Generation
     ↓
Advanced Retrieval
     ↓
Hybrid Search
     ↓
Reranking
     ↓
Multimodal RAG
```

## Reference

This project follows a structured RAG learning series covering topics from introductory RAG architecture through advanced retrieval, hybrid search, reranking, and multimodal RAG.
