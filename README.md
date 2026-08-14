# XYZ

<p align="center">

**Open-source AI models for local use**

[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Open Source](https://img.shields.io/badge/Open--Source-Yes-blue.svg)]()
[![Local AI](https://img.shields.io/badge/Local-AI-orange.svg)]()

</p>

---

## About

**XYZ** is an open-source family of AI models focused on **local inference, programming and general text tasks**.

The main goal of the project is to create useful AI models that can run locally on consumer hardware without requiring cloud APIs.

The project focuses on:

- local AI
- code generation
- instruction following
- efficient inference
- low VRAM usage
- open-source development

---

# Model Family

XYZ currently focuses on three models:

| Model | Parameters | Target Hardware | Main Focus | Status |
|---|---:|---|---|---|
| **XYZ-Coder Mini** | 7B | 4–6 GB VRAM | Lightweight coding | Planned |
| **XYZ-Coder-1** | 118M | 4–8 GB VRAM | Compact coding | In development |
| **XYZ-Coder-2** | ~1B | 6–8 GB VRAM | Local coding | Planned |

> Model sizes and hardware requirements may change during development.

---

# Models

## XYZ-Coder Mini

A lightweight version designed for older GPUs and laptops with limited VRAM.

The main goal is to provide a useful coding assistant on hardware with around **4–6 GB of VRAM**.

### Focus

- Code generation
- Code completion
- Basic programming questions
- Local inference
- Low memory usage

---

## XYZ-Coder-1

The first experimental XYZ-Coder model.

### Specifications

| Parameter | Value |
|---|---:|
| Parameters | **118,056,960 (~118M)** |
| Architecture | Decoder-only Transformer |
| Layers | **14** |
| Attention heads | **12** |
| Embedding size | **768** |
| Context length | **512 tokens** |
| Vocabulary | **24,000 BPE** |
| Dropout | **0.1** |

### Training Data

Current training direction:

| Category | Target |
|---|---:|
| 🔥 Code | **65%** |
| 🧠 Dialogue | **20%** |
| 📚 Knowledge | **15%** |

The current training dataset contains approximately **923M+ tokens**.

The current model is trained from scratch using a custom PyTorch training pipeline.

---

## XYZ-Coder-2

The next generation of XYZ-Coder.

Target size:

**~1 billion parameters**

The goal of XYZ-Coder-2 is to provide significantly better:

- code generation
- instruction following
- context understanding
- programming explanations
- local coding performance

Development details will be published as the model progresses.

---

# Training

XYZ models are built around Transformer architectures and trained using PyTorch.

Current training pipeline includes:

- AdamW
- BF16 mixed precision
- scaled dot-product attention
- cosine learning rate
- learning-rate warmup
- gradient clipping
- automatic batch-size selection
- checkpointing
- custom BPE tokenizer

---

# Current Training Hardware

XYZ-Coder-1 is currently being developed on consumer hardware.

```text
GPU: NVIDIA RTX 4060 Ti 16GB
CPU: Intel Core i5-12400
RAM: 32GB
