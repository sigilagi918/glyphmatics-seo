---
license: mit
tags:
- vision-encoder
- vision-language-model
- video
- self-supervised
- glyphs
- symbolic
- deterministic
language:
- multilingual
demo:
- url: https://huggingface.co/spaces/Nine1Eight/vil-glyphmatic-demo
---

# vil-encoder-v1.1  
## Glyphmatic Vision Encoder (GVL-P Trained)

**Author:** Matthew Blake Ward (Nine1Eight)  
**Location:** Tulsa, Oklahoma, USA  

---

## 🔴 Live Demo (Integrated Space)

👉 **https://huggingface.co/spaces/Nine1Eight/vil-glyphmatic-demo**

This Space uses **vil-encoder-v1.1** to encode:

- Glyph collages (images)
- Glyph evolution sequences (videos)
- Temporal execution structure

---

## Model Overview

`vil-encoder-v1.1` is a **vision encoder** trained using **GVL-P self-supervision**.

It does **not** perform language modeling.  
It produces **execution-aware embeddings** from glyph visuals.

---

## Architecture

- Vision Transformer–style encoder
- Temporal aggregation head
- Deterministic forward pass
- No tokenizer
- No vocabulary
- No sampling

Inputs:
- Glyph collages
- Glyph video frame stacks

Outputs:
- Dense embeddings aligned to glyph execution structure

---

## Training

- **Training regime:** GVL-P v1.1
- **Supervision:** Self-synthesized
- **Labels:** None
- **Data sources:** Glyph-rendered images & videos
- **Canon:** Locked (111 glyph index space)

---

## Intended Use

- Vision–language models using glyph IR
- Multimodal reasoning
- Video pretraining
- Execution-aware embedding research
- Adapter / LoRA fine-tuning

---

## Limitations

- Encoder only (not a full VLM)
- Requires glyph-based inputs
- No natural-language decoding
- Canon is immutable

---

## Relationship to VIL

This encoder is designed to plug into:

👉 **Nine1Eight/vil-canonical-glyph-system**

It is **canon-bound** and cannot be retrained on altered glyph sets.

---

## Security

- No execution of decoded content
- No file system access
- No system calls

---

## Citation

If you use this model, cite:

- VIL Canonical Glyph System
- GVL-P v1.1
- vil-encoder-v1.1

---

## Author

Matthew Blake Ward (Nine1Eight)  
Tulsa, Oklahoma, USA
# SigilAGI
