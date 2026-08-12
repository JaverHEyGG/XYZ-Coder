# XYZ

<p align="center">
  <img src="assets/banner.png" alt="XYZ">
</p>

<h3 align="center">Open-source AI models built for local use</h3>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-green.svg"></a>
  <a href="#"><img src="https://img.shields.io/badge/Models-XYZ-blue.svg"></a>
  <a href="#"><img src="https://img.shields.io/badge/Local-AI-orange.svg"></a>
  <a href="#"><img src="https://img.shields.io/badge/Open--Source-Yes-purple.svg"></a>
</p>

---

## About XYZ

**XYZ** is an open-source family of AI models designed for **local inference, programming, and general text tasks**.

The main goal of the project is to create powerful models that can run locally on consumer hardware, including systems with limited VRAM.

The project is being developed from scratch with a focus on:

- local AI
- code generation
- instruction following
- efficient inference
- low VRAM usage
- open-source development

---

# Model Family

XYZ is designed as a family of models with different sizes and hardware targets.

| Model | Parameters | Target Hardware | Main Focus | Status |
|---|---:|---|---|---|
| **XYZ-Coder Mini** | 7B | 4–6 GB VRAM | Lightweight coding | Planned |
| **XYZ-Coder-1** | 118M | 4–8 GB VRAM | Experimental / compact | In development |
| **XYZ-Coder-2** | ~1B | 6–8 GB VRAM | Local coding | Planned |
| **XYZ-Coder-3** | ~3B | 8–12 GB VRAM | Coding | Planned |
| **XYZ-Coder-4** | ~7B | 8–16 GB VRAM | Advanced coding | Planned |
| **XYZ-Coder-5** | ~16B | 12–16 GB VRAM | High-performance local coding | Planned |
| **XYZ-Coder-6** | ~32B | 16 GB+ / aggressive quantization | Maximum local performance | Planned |

> Model sizes and hardware requirements may change as the architecture and quantization methods evolve.

---

# Why XYZ?

Most large AI models require expensive hardware or cloud services.

XYZ focuses on a different goal:

> **Bring powerful AI closer to the user's own computer.**

The project aims to make different model sizes available for different hardware configurations.

### Example

```text
4 GB VRAM
    ↓
XYZ Mini

8 GB VRAM
    ↓
XYZ 1B / 3B

12 GB VRAM
    ↓
XYZ 7B / 16B quantized

16 GB VRAM
    ↓
XYZ 16B / 32B heavily quantized
