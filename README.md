# Medical_chatbot
# 🩺 Medical Chatbot using DeepSeek-RL + LoRA

This project implements a medical chatbot powered by **DeepSeek-RL**, fine-tuned using **LoRA (Low-Rank Adaptation)** on a domain-specific medical reasoning dataset. The chatbot is designed to provide intelligent, context-aware responses to medical queries.

---

## 🚀 Project Goals

- Fine-tune large language models efficiently using **LoRA**, reducing computational cost.
- Leverage instruction-tuned medical datasets for better reasoning capabilities.
- Build a reliable AI-based medical assistant that can be deployed in real-world settings.

---

## 🧠 Model Architecture

- **Base Model:** `DeepSeek-RL` (via Hugging Face)
- **Fine-tuning Method:** `LoRA` (via `peft` library)
- **Dataset:** `FreedomIntelligence/medical-01-reasoning-SFT`
- **Tokenizer:** `AutoTokenizer` from Hugging Face
- **Key Libraries:** 
  - `transformers`
  - `datasets`
  - `peft` (for LoRA)
  - `huggingface_hub`
  - `Google Colab`

---

## ⚙️ Why LoRA?

LoRA enables efficient fine-tuning of large models by injecting trainable rank decomposition matrices into each layer of the Transformer. This results in:

- **Up to 95% parameter reduction**
- **Faster training on limited hardware (e.g. Google Colab)**
- **Maintains or even improves performance on downstream tasks**

---


