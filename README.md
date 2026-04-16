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

![CI/CD](https://github.com/nhatminh-115/PPE-Detection/actions/workflows/ci-cd-pipeline.yml/badge.svg)

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
- **AI / ML:** `PyTorch` `YOLO` `timm` `ONNX Runtime` `LangGraph` `ChromaDB`
- **MLOps / Cloud:** `Docker` `Terraform` `AWS (EC2, S3)` `MLflow` `GitHub Actions`
- **Backend / Data:** `Python` `FastAPI` `Supabase` `MQTT`

---

## Certifications
- **Deep Learning Specialization** — DeepLearning.AI
- **MLOps Specialization** — Duke University

---

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/nnminh115/)
