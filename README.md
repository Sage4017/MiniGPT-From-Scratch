# MiniGPT — GPT from Scratch

A character-level GPT language model implemented from scratch in PyTorch,
following Andrej Karpathy's Neural Networks: Zero to Hero series.

## What I built

- Character-level tokenizer
- Token + positional embeddings
- Causal self-attention
- Multi-head self-attention
- Feed-forward networks
- Layer normalization
- Residual connections
- Dropout
- AdamW optimization
- Autoregressive text generation

## Architecture

Input
  ↓
Token Embedding + Positional Embedding
  ↓
6 Transformer Blocks
  ↓
LayerNorm
  ↓
Linear Language Model Head
  ↓
Next-character prediction

## Model Configuration

- Context length: 64
- Embedding dimension: 384
- Attention heads: 6
- Transformer layers: 6
- Dropout: 0.2
- Batch size: 256
- Learning rate: 3e-4
- Training iterations: 5000

## Results

The model was trained on a Shakespeare text corpus and generated
Shakespeare-like dialogue from scratch.

Example:

> Fourth, thou till I will whether I was razed...

[put your generated sample here]

## How to run

```bash
pip install torch
python script.py
