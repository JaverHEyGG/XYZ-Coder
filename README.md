# XYZ-Coder-1 118M

<p align="center">

**Небольшая open-source языковая модель для программирования и работы с текстом**

[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Parameters](https://img.shields.io/badge/Parameters-118M-blue.svg)]()
[![Architecture](https://img.shields.io/badge/Architecture-Transformer-orange.svg)]()
[![VRAM](https://img.shields.io/badge/VRAM-16GB-purple.svg)]()

</p>

---

## О модели

**XYZ-Coder-1 118M** — компактная decoder-only Transformer-модель, обучаемая с нуля.

Основная задача модели — локальная работа с программированием при небольшом потреблении ресурсов.

### Основные характеристики

| Параметр | Значение |
|---|---:|
| Параметры | **118,056,960 (~118M)** |
| Архитектура | Decoder-only Transformer |
| Layers | **14** |
| Attention heads | **12** |
| Embedding size | **768** |
| Context length | **512 токенов** |
| Vocabulary | **24,000 BPE** |
| Dropout | **0.1** |
| Основной фокус | **Programming / Code** |

---

## Данные

Модель обучается на смешанном корпусе:

| Категория | Целевая доля |
|---|---:|
| 🔥 Code | **65%** |
| 🧠 Dialogue | **20%** |
| 📚 Knowledge | **15%** |

Текущая версия корпуса содержит примерно:

**653M+ токенов**

Целевой объём:

**1B токенов**

---

## Примеры

### Python

**Prompt**

```text
Напиши Hello World на Python
