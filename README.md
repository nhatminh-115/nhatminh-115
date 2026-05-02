# Hi, I'm Minh

**AI Engineer | Final-year Robotics & AI @ UEH**

I build production-grade AI systems — from fine-tuning and serving LLMs to deploying real-time computer vision pipelines on the cloud.

---

## Featured Projects

### [PPE Detection](https://github.com/nhatminh-115/PPE-Detection)
*Real-Time PPE Compliance Monitoring — Computer Vision · MLOps · LLM Reporting*

- **Detection:** YOLO11s + YOLO26l WBF ensemble + ByteTrack + Box EMA for stable multi-person tracking
- **Classification:** EfficientNetV2-B0 ONNX FP32 (7.46ms vs 45ms PyTorch — 6x speedup, F1=0.92) for small boxes; SigLIP SO400M ONNX FP16 (3.2x GPU speedup, 4x size reduction) for large boxes
- **State Management:** Hysteresis FSM + Classify Lock to suppress alert fatigue and reduce redundant GPU inference
- **Data Flywheel:** Closed-loop retraining via S3 + EC2 Spot + MLflow; drift triggered by 7-day rolling human disagreement rate
- **Reporting:** LangGraph 4-agent pipeline + ChromaDB RAG on Thông tư 25/2022 — daily compliance reports with regulation citations
- **Infra:** Terraform (AWS), Docker, GitHub Actions CI/CD, DagsHub MLflow

### [ReframeBot](https://github.com/nhatminh-115/ReframeBot)
*CBT-Oriented Mental Health Chatbot — Fine-tuned Llama 3.1 8B*

- **Fine-tuning:** SFT + DPO on Llama 3.1 8B via PEFT/LoRA; AWQ 4-bit quantization reduces VRAM to ~5.4 GB
- **Serving:** vLLM + PagedAttention — p50 latency 2.6s, TTFT 1.11s, ~39 tok/s
- **Guardrail Router:** DistilBERT 3-class classifier (CBT / Crisis / Out-of-scope) — 88.3% accuracy on out-of-domain eval set
- **Infra:** Dockerized two-container stack (vLLM + FastAPI); RAG grounding via ChromaDB; models published on HuggingFace

### [GreenCalyx AI](https://github.com/nhatminh-115/GreenCalyx_AI)
*Logistics ESG Scoring Tool — CAIEC Competition*

- **Pipeline:** LangGraph agent parses 5 trade document types (CI, PL, BL/AWB, TDS, PPWR) via Groq Llama-4-Scout vision
- **Emissions:** CO2e calculation aligned with GLEC Framework v3.2 / ISO 14083; sea routing via searoute-py
- **Output:** ESG score (0–100) with GREEN/YELLOW/RED lane classification; results logged to Supabase

### [Digital Twin — Environment Monitoring](https://github.com/nhatminh-115/IoT-DigitalTwin-Backend)
*Graduation Internship @ UEH Campus V · In Progress*

- LSTM one-step forecaster + Autoencoder anomaly detection on 8 sensor nodes
- DataQualityGate pipeline: flatline detection, z-score outlier removal, linear interpolation
- Telegram bot with Groq Llama 3.3 70B assistant and intent-based context routing
- Real-time Unity 3D visualization deployed on live VPS

---

## Tech Stack

- **LLM & Fine-tuning:** `PyTorch` `Transformers` `PEFT/LoRA` `TRL (SFT/DPO)` `LangGraph` `ChromaDB` `Groq`
- **Model Serving & Optimization:** `vLLM` `AWQ` `ONNX Runtime (FP32/FP16/INT8)`
- **Computer Vision:** `YOLO` `EfficientNetV2` `SigLIP` `ByteTrack` `OpenCV`
- **MLOps & Cloud:** `Docker` `Terraform` `AWS (EC2, S3)` `MLflow` `GitHub Actions`
- **Backend & Data:** `FastAPI` `PostgreSQL` `Supabase` `Python`

---

## Certifications

- **Deep Learning Specialization** — DeepLearning.AI
- **MLOps Specialization** — Duke University

---

*Ours is the fury.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/nnminh115/)
