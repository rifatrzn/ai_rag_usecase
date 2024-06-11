# RAG NVIDIA Project

## Overview

This project demonstrates the use of various tools and techniques for Retrieval-Augmented Generation (RAG), query routing, and function calling with Groq and LangChain. The implementation includes setting up data loading, embedding models, vector indexing, and query engines.

## Installation

Install the necessary packages:

```bash
!pip install langchain_nvidia_ai_endpoints
!pip install langchain-community langchain-text-splitters faiss-cpu
!pip install llama-index-llms-groq
!pip install llama-index llama-index-llms-huggingface llama-index-embeddings-huggingface transformers accelerate bitsandbytes llama-index-readers-web matplotlib flash-attn
!pip install openai