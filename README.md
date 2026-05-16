# ALAF: Adaptive Legal Arbitration Framework

# Code will be updated after acceptance of the paper.

Official implementation for the paper:

**“ALAF: An Adaptive Legal Arbitration Framework for Near-Zero Hallucination Regulatory Compliance Checking”**

## Overview

ALAF is a hybrid legal AI framework combining:

- Deterministic rule-based validation
- Constrained LLM inference
- Temporal Retrieval-Augmented Generation (RAG)
- Arbitration-based hallucination suppression

The system is designed for regulatory compliance checking on legal contracts while minimizing hallucinated clause classifications.

---

## Key Features

- Hybrid rule-engine + LLM routing
- Temporal RAG pipeline using live regulatory feeds
- Structured JSON prompt contracts
- Confidence-threshold arbitration
- Hallucination-aware evaluation pipeline

---

## Architecture

![Architecture](screenshots/architecture.png)

---

## Dataset

This project uses the CUAD dataset:

- CUAD Paper: https://arxiv.org/abs/2103.06268
- CUAD Dataset: https://huggingface.co/datasets/theatticusproject/cuad

---

## Model Configuration

Primary model:
- `llama3-70b-8192` via Groq API

Groq Documentation:
- https://console.groq.com/docs/model/llama3-70b-8192

Generation Parameters:

```yaml
temperature: 0.0
top_p: 0.1
response_format: json
