
## Sentinel-AI: Multi-Class LLM Guardrail

Sentinel-AI is a proactive security gateway designed to intercept, analyze, and classify user prompts before they reach a Large Language Model (LLM). Built for the 2026 security landscape, it moves beyond simple "keyword blocking" to deep semantic understanding of intent.

## 🚀 The Problem

As LLMs are integrated into enterprise workflows, they face sophisticated "Natural Language Attacks." Standard filters often fail to distinguish between complex academic queries and malicious injections. Sentinel-AI solves this by using a fine-tuned Transformer model to categorize intent with high precision.

## 🛠️ Key Features

Multi-Class Classification: Unlike binary filters, this system categorizes inputs into four distinct buckets:

- ✅ Benign: Legitimate, safe user queries.

- 🛡️ Jailbreak: Attempts to bypass safety logic via roleplay or persona adoption.

- 📂 Leakage: Intent to extract internal system prompts or proprietary instructions.

- 🚫 Harmful: Direct requests for dangerous, illegal, or toxic content.

- Real-Time Dashboard: A Gradio-powered interface for live security monitoring.

- Transformer-Based: Built on DeBERTa-v3-small, utilizing disentangled attention for superior adversarial detection.
## 📊 Evaluation Data

The model was trained on a synthesized blend of:

- Alpaca-Cleaned: For high-quality benign instruction following.

- Deepset Prompt-Injections: For real-world jailbreak patterns.

- Adversarial Synthetic Sets: Targeted data for prompt leakage and cybercrime detection.

## Results

<img width="1893" height="389" alt="image" src="https://github.com/user-attachments/assets/ed849324-02b6-47f2-a919-a3b9eecdaa56" />


## 🛡️ Security Disclaimer
This tool is intended for research and as a component of a "defense-in-depth" strategy. No guardrail is 100% impenetrable; it should be used in conjunction with output filtering and robust system architectures.
