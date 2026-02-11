👨‍💻 Author
Yashwi Pandey

# RAG-Based Question Answering System  
### Agentic AI Lab Assignment

---

## Project Overview

This project implements a **Retrieval Augmented Generation (RAG)** system that enables question answering from custom documents. 

Traditional Large Language Models (LLMs) rely only on pre-trained knowledge and may generate hallucinated responses. This system improves reliability by retrieving relevant document chunks from a vector database and using them to generate grounded, context-aware answers.

The project demonstrates the complete RAG pipeline including document loading, text chunking, embeddings, vector storage, retrieval, and answer generation.

---

## Problem Statement

Large Language Models cannot accurately answer questions from private or domain-specific documents because they do not have access to that data.  

The objective of this project is to build a RAG-based system that:
- Stores document knowledge in a vector database
- Retrieves relevant information based on user queries
- Generates accurate responses using retrieved context

This reduces hallucination and improves answer quality.

---

## Dataset / Knowledge Source

- **Type of Data:** PDF 
- **Source:** Publicly available 
- **Domain:** Artificial Intelligence

The documents are processed and converted into vector embeddings for semantic retrieval.

---

## RAG Architecture

The system follows the below pipeline:
User Query
↓
Embedding Model
↓
Vector Database (FAISS / Chroma)
↓
Retriever
↓
Language Model (LLM)
↓
Final Response


This architecture ensures that responses are generated based on retrieved document context instead of relying solely on pretrained model knowledge.

---

## Text Chunking Strategy

- **Chunk Size:** 500 characters  
- **Chunk Overlap:** 50 characters  

### Reason for Strategy

Chunking divides large documents into smaller meaningful segments for efficient processing and retrieval.  
Overlap ensures contextual continuity between chunks and improves retrieval performance by preventing loss of important information across chunk boundaries.

---

## Embedding Details

- **Embedding Model Used:** `sentence-transformers/all-MiniLM-L6-v2`

### Reason for Selecting the Model

- Lightweight and computationally efficient  
- Provides good semantic similarity performance  
- Works effectively with FAISS / Chroma  
- Suitable for small-to-medium scale RAG implementations  

---

## Vector Database

- **Vector Store Used:** FAISS / Chroma  

### Why This Vector Store?

- Fast similarity search  
- Efficient vector indexing  
- Easy local setup  
- Widely adopted in RAG systems  

---

## Tools & Libraries Used

- Python  
- LangChain  
- FAISS / Chroma  
- Sentence Transformers  
- HuggingFace Transformers  
- PyPDF  
- Google Colab  

---

## How to Run the Project

1. Open `RAG_Agentic_AI.ipynb` in Google Colab.  
2. Install required dependencies:

    pip install langchain faiss-cpu sentence-transformers pypdf chromadb transformers torch

3. Upload the required document(s).  
4. Run all cells sequentially.  
5. Enter queries to retrieve answers from the document knowledge base.

---

## Sample Queries

The notebook demonstrates at least three test queries, such as:

- What is Artificial Intelligence?  
- Explain supervised learning.  
- What are the applications of AI?  

Each query retrieves relevant document chunks and generates a context-aware response.

---

## Future Improvements

- Semantic chunking techniques  
- Hybrid search (BM25 + Vector Search)  
- Reranking models  
- Metadata filtering  
- Streamlit / Gradio UI integration  
- Support for multiple documents  

---

## Conclusion

This project successfully demonstrates how Retrieval Augmented Generation enhances answer reliability by grounding responses in document-based knowledge.

By integrating document retrieval with language model generation, the system produces accurate, context-aware, and reliable answers.

---
