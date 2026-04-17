# Hi, I'm Minh 👋
**AI Engineer | Final-year Robot-AI @ UEH**

I build AI systems — from training deep learning models to architecting real-time inference pipelines on the cloud.

---

## Featured Projects

### [PPE Detection](https://github.com/nhatminh-115/PPE-Detection)
*Real-Time PPE Compliance Monitoring System*

- **Detection:** YOLO11s + YOLO26l WBF ensemble (weights=[2,1]) + ByteTrack + Box EMA for stable tracking
- **Classification:** EfficientNetV2-B0 (F1=0.92, ONNX 7.46ms vs 45ms PyTorch — 6x speedup) for small boxes; SigLIP SO400M zero-shot for large boxes
- **State Management:** Hysteresis FSM + Classify Lock to suppress alert fatigue and reduce redundant GPU inference
- **Data Flywheel:** Closed-loop retraining via S3 versioning + EC2 Spot + MLflow; drift triggered by 7-day rolling human disagreement rate
- **Reporting:** LangGraph 4-agent pipeline + ChromaDB RAG on Thông tư 25/2022 → daily compliance reports with regulation citations
- **Infra:** Terraform (AWS), Docker, GitHub Actions CI/CD, Docker Hub, DagsHub MLflow

### [ReframeBot](https://github.com/nhatminh-115/ReframeBot)
*CBT-Oriented Mental Health Chatbot — Fine-tuned Llama 3.1 8B*

- **Fine-tuning:** SFT + DPO on Llama 3.1 8B via PEFT/LoRA; DPO adapter improves response preference alignment
- **Quantization:** AWQ 4-bit (autoawq) — VRAM footprint ~5.4 GB on RTX 5070; exported and published on Hugging Face
- **Serving:** vLLM + PagedAttention via OpenAI-compatible API; p50 latency 3.3s, TTFT 1.09s, ~54 tok/s
- **Guardrail Router:** DistilBERT 3-class classifier (CBT / Crisis / Out-of-scope) — Accuracy 91.1%
- **Infra:** Dockerized two-container stack (vLLM + FastAPI); RAG grounding via ChromaDB

### [GreenCalyx AI](https://github.com/nhatminh-115/GreenCalyx_AI)
*Logistics ESG Scoring Tool — CAIEC Competition*

- **Pipeline:** LangGraph agent parses 5 trade document types (CI, PL, BL/AWB, TDS, PPWR) via Groq Llama-4-Scout vision
- **Emissions:** CO2e calculation aligned with GLEC Framework v3.2 / ISO 14083; sea routing via searoute-py (accounts for Malacca, Suez, Panama)
- **Output:** ESG score (0–100) with GREEN/YELLOW/RED lane classification and natural-language explanation; results logged to Supabase


### [Digital Twin — Environment Monitoring](https://github.com/nhatminh-115/IoT-DigitalTwin-Backend) *(In Progress)*
*Graduation Internship @ UEH Campus V*

- LSTM one-step forecaster + Autoencoder anomaly detection on 8 sensor nodes
- DataQualityGate pipeline: flatline detection, z-score outlier removal, linear interpolation
- Telegram bot with AI assistant (Groq Llama 3.3 70B) and intent-based context routing

---

## Tech Stack
- **LLM & Fine-tuning:** `PyTorch` `Transformers` `PEFT/LoRA` `TRL (SFT/DPO)` `LangGraph` `ChromaDB` `Groq`
- **Model Serving & Optimization:** `vLLM` `AWQ (autoawq)` `ONNX Runtime`
- **Computer Vision:** `YOLO` `OpenCV`
- **MLOps & Cloud:** `Docker` `Terraform` `AWS (EC2, S3)` `MLflow` `GitHub Actions`
- **Backend & Data:** `FastAPI` `PostgreSQL` `Supabase` `Python`

---

## Certifications
- **Deep Learning Specialization** — DeepLearning.AI
- **MLOps Specialization** — Duke University

---
*Ours is the fury.*


[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/nnminh115/)
