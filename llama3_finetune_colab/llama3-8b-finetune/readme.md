# Fine-Tuning LLaMA-3 Model with LoRA using Unsoth

## Overview

This project demonstrates the fine-tuning of the LLaMA-3 model using Low-Rank Adaptation (LoRA) techniques with the `unsloth` library. The goal is to leverage efficient memory usage and enhance model performance using 4-bit quantization and advanced training configurations.

## Installation

Ensure you have the necessary dependencies installed. Depending on your GPU, you may need different packages:

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

This project showcases the powerful integration of unsloth, LoRA, and the LLaMA-3 model to create an efficient and high-performing language model. Feel free to explore and modify the setup to suit your needs.