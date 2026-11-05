# LNER - Lightweight Language Model for Code Completion

LNER is a GPT-style language model built with PyTorch. It generates code completions using custom-trained transformer models for Python and C++.

## Features

- Custom byte-level BPE tokenizer
- Decoder-only Transformer with causal self-attention
- GPU-accelerated training with CUDA
- Lazy dataset loading
- Cross-device inference (CUDA, Apple MPS, CPU)
- PySide6 desktop code editor
- Syntax highlighting and ghost-text suggestions
- Background completion generation

## Model Architecture

| Parameter | Value |
|---|---:|
| Transformer layers | 6 |
| Attention heads | 8 |
| Model dimension | 256 |
| Feed-forward dimension | 1,024 |
| Vocabulary size | 12,000 |
| Context length | 256 tokens |

## Requirements

- Python
- PyTorch
- Hugging Face Tokenizers
- PySide6
- psutil

Install dependencies:

```bash
pip install torch tokenizers PySide6 psutil
```

## Overview

LNER was built to explore language model development, from tokenization and transformer implementation to training and integration.

It is designed for short code completions rather than complex code generation.

## Future Work

- Expand training datasets
- Improve completion quality
- Add performance benchmarks
- Optimize inference speed
