# Rulu2

Rulu is a from-scratch language-model project. This repository contains the Rulu V7 1B-class model metadata, training corpus, Ollama configuration, and build tooling.

## Model

- Version: Rulu V7
- Parameters: ~1.028B
- Architecture: Llama-style transformer
- Hidden size: 2048
- Layers: 20
- Attention heads: 8
- FFN size: 5632
- Context: 512 tokens
- Vocabulary: 257 byte-level tokens
- Weights: F16 GGUF
- Pretrained base: none

## Topics

The training corpus keeps the previous Rulu material and adds programming/software, game development, AI/ML, databases, networking, operating systems, cybersecurity, mathematics, science, biology, chemistry, physics, astronomy, history, archaeology, geography, philosophy, psychology, literature, art, music, food, sports, language, nature, travel, everyday life, communication, creativity, and reasoning.

## Ollama

```bash
ollama create rulu -f ./Modelfile
ollama run rulu
```

The large GGUF is distributed separately because GitHub's normal repository file path has strict size limits. The `MODEL_SHA256.txt` file records the expected checksum for the local model artifact.
