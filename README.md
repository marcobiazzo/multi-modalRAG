# Multi-modal RAG with Gemini Pro

This codelab demonstrates how to build a question-answering system using multi-modal retrieval augmented generation (RAG) with Gemini Pro.

**Last updated:** June 27, 2024

**Authors:** Bhushan Garware, Aditya Rane, Leonid Kuligin

## Introduction

This codelab explores the concept of multi-modal RAG, which enhances traditional RAG systems by incorporating visual information from images. This approach allows for a deeper understanding of information and enables more accurate and comprehensive answers to user queries, especially when dealing with documents containing graphs, diagrams, and other visual elements.

### What is RAG?

Retrieval Augmented Generation (RAG) combines large language models (LLMs) with external knowledge sources to provide more accurate, relevant, and adaptable responses.

### Why Multi-Modal?

Multi-modal RAG leverages both text and image data to provide a more comprehensive understanding of information. This is crucial in today's data-rich environment where documents often combine text and images to convey information effectively.

### Two Options for Multi-modal RAG

* **Multimodal Embeddings:** This approach uses a single model to generate embeddings for both text and images, allowing for seamless searching and retrieval of both modalities.
* **Text Embeddings:** This method uses an LLM to generate text summaries of images, which are then used for retrieval alongside text embeddings.

### What is Multi-Vector Retriever?

Multi-vector retrieval enhances RAG by using summaries of document sections to retrieve original content for answer synthesis. This is particularly useful for documents containing tables, graphs, and charts.

## What you'll build

This codelab guides you through building a question-answering system using Gemini Pro that can effectively extract information from documents containing complex visuals.

**Use case:** Developing a question-answering system using Gemini Pro for documents with complex graphs or diagrams.

**Steps:**

1. **Data loading:** Load data using LangChain document loaders.
2. **Text summarization:** Generate text summaries using Google's `gemini-pro` model.
3. **Image summarization:** Generate image summaries using Google's `gemini-pro-vision` model.
4. **Retrieval:** Create multi-vector retrieval using Google's `textembedding-gecko` model with Croma Db as the vector store.
5. **Question answering:** Develop a multi-modal RAG chain for question answering.

This codelab provides a hands-on experience in building a multi-modal RAG system, enabling you to leverage the power of Gemini Pro for advanced question answering and information extraction tasks.
