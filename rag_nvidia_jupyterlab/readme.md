# Nvidia NIM Demo with LangChain and Gradio in Jupyter Lab

## Overview

This project demonstrates the integration of Nvidia NIM with LangChain and Gradio to create a document question-answering system. The system allows users to ask questions about a set of documents and receive accurate responses based on the content of those documents.

## Installation

To get started, ensure you have the necessary dependencies installed. Depending on your GPU, you may need different packages:

```bash
import torch
major_version, minor_version = torch.cuda.get_device_capability()

# Must install separately since Colab has torch 2.2.1, which breaks packages
!pip install "unsloth[colab-new] @ git+https://github.com/unslothai/unsloth.git"

if major_version >= 8:
    # Use this for new GPUs like Ampere, Hopper GPUs (RTX 30xx, RTX 40xx, A100, H100, L40)
    !pip install --no-deps packaging ninja einops flash-attn xformers trl peft accelerate bitsandbytes
else:
    # Use this for older GPUs (V100, Tesla T4, RTX 20xx)
    !pip install --no-deps xformers trl peft accelerate bitsandbytes
```

## Running the Application

-Ensure your environment is set up and dependencies are installed.
-Load the environment variables for your Nvidia API key.
-Run the document ingestion and vector store creation script.
-Use the Gradio interface to embed documents and ask questions.


This project showcases the powerful integration of Nvidia NIM, LangChain, and Gradio to create an interactive document question-answering system in local environment with jupyter lab. Feel free to explore and modify the setup to suit your needs.
