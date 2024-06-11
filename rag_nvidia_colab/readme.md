# RAG with Nvidia NIM and LangChain HYDE

## Overview

This rag_gen_hyde.ipynb demonstrates the use of Nvidia NIM and LangChain for Retrieval-Augmented Generation (RAG). The implementation involves loading documents, creating a FAISS vector store, and answering questions based on the context of the web documents using Nvidia NIM.

## Installation

Ensure you have the necessary dependencies installed:

```bash
!pip install langchain_nvidia_ai_endpoints
!pip install langchain-community langchain-text-splitters faiss-cpu
!pip install openai

```


# Document Question-Answering with Nvidia NIM and Gradio

## Overview

This rag_gradio.ipynb demonstrates the use of Nvidia NIM and Gradio for creating an interactive question-answering system based on a set of documents. The system loads documents, creates a FAISS vector store, and answers user queries with relevant context from the documents.

## Installation

Ensure you have the necessary dependencies installed:

```bash
!pip install langchain_nvidia_ai_endpoints
!pip install langchain-community langchain-text-splitters faiss-cpu
!pip install gradio
!pip install python-dotenv
```

These two projects demonstrate how to use Nvidia NIM with LangChain and Gradio to build advanced question-answering systems based on document context. Feel free to explore and modify the setup to suit your needs.

License
This project is licensed under the MIT License.

This `README.md` file provides a clear and comprehensive guide for setting up and running each project individually.
