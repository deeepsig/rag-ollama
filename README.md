# RAG Using LangChain, ChromaDB, Ollama and Gemma 7b

![QA_RAG](https://github.com/deeepsig/rag-ollama/assets/81250703/de18df3d-039c-4fcd-94cd-35cfdf54930a)

## About

RAG serves as a technique for enhancing the knowledge of Large Language Models (LLMs) with additional data.

While LLMs possess the capability to reason about diverse topics, their knowledge is restricted to public data up to a specific training point. To develop AI applications capable of reasoning about private or post-cutoff date data, it becomes necessary to supplement the model's knowledge with specific information. This process of integrating relevant information into the model prompt is termed Retrieval Augmented Generation (RAG).

A typical RAG application comprises two main components: Indexing and Retrieval and Generation.

Indexing plays a crucial role in facilitating efficient information retrieval. Initially, data is extracted from private sources and partitioned to accommodate long text documents while preserving their semantic relations. Subsequently, this partitioned data is stored in a vector database, such as ChromaDB or Pinecone. In our case, we utilize ChromaDB for indexing purposes.

Next, in the Retrieval and Generation phase, relevant data segments are retrieved from storage using a Retriever. These segments, along with the user query, are then incorporated into the model prompt. Our approach employs an open-source local LLM, Gemma 7b, with the assistance of Ollama.

## Objective

In this notebook we implement a simple RAG system using LangChain, ChromaDB, Ollama and the Gemma 7b model.

## Kaggle Site
https://www.kaggle.com/code/deeepsig/rag-using-langchain-chromadb-ollama-and-gemma-7b/notebook

