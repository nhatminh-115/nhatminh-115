<p align="center">
  <img src="assets/minh-profile-banner.svg" alt="Nhat Minh — AI / ML Engineer" width="100%" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/nnminh115/"><img src="https://img.shields.io/badge/LinkedIn-connect-4b3b2a?style=flat-square&logo=linkedin&logoColor=d8bd8b" alt="LinkedIn" /></a>
  <a href="mailto:nhatminhvcst115@gmail.com"><img src="https://img.shields.io/badge/Email-contact-4b3b2a?style=flat-square&logo=gmail&logoColor=d8bd8b" alt="Email" /></a>
  <a href="https://github.com/nhatminh-115"><img src="https://img.shields.io/badge/GitHub-nhatminh--115-4b3b2a?style=flat-square&logo=github&logoColor=d8bd8b" alt="GitHub" /></a>
</p>

<p align="center">
  <strong>Ho Chi Minh City, Vietnam</strong> &nbsp;·&nbsp; B.Eng. Robotics &amp; Artificial Intelligence, UEH &nbsp;·&nbsp; Expected Mar 2027
</p>

---

## About

I build AI systems across **computer vision, LLM applications, and applied machine learning**. My work focuses on the engineering between a model and a usable system: data quality, evaluation, inference optimization, backend integration, and deployment.

I enjoy investigating why models behave the way they do, measuring what actually improves, and turning validated components into systems that can be operated and maintained.

## Selected Work

### [SentinelVision](https://github.com/nhatminh-115/SentinelVision-Showcase) · Computer Vision & MLOps

Real-time PPE compliance monitoring for construction and industrial environments.

- **Detection and tracking:** YOLO ensemble, Weighted Boxes Fusion, ByteTrack, and temporal smoothing for multi-person tracking.
- **Dual-path classification:** EfficientNetV2-B0 ONNX for small person boxes; SigLIP SO400M ONNX FP16 for larger boxes.
- **Inference optimization:** EfficientNet ONNX reaches **7.46 ms CPU latency** with **F1 = 0.92** on the small-box route; SigLIP ONNX FP16 delivers **3.2× GPU speedup** over its PyTorch FP32 baseline.
- **Human-in-the-loop MLOps:** versioned human-confirmed labels, disagreement monitoring, gated EC2 Spot retraining, and MLflow/DagsHub artifact tracking.

### [ReframeBot](https://github.com/nhatminh-115/ReframeBot) · LLM Systems & Evaluation

A CBT-oriented chatbot for university students, built around local LLM serving, safety routing, and retrieval evaluation.

- Fine-tuned Llama 3.1 8B with **SFT + DPO**, then applied **AWQ 4-bit quantization**.
- Served through a Dockerized **vLLM + FastAPI** stack with PagedAttention, continuous batching, and SSE streaming.
- Added a DistilBERT guardrail router for CBT, crisis, and out-of-scope inputs, with explicit crisis-signal handling.
- Evaluated retrieval quality with **RAGAS** and traced application behavior with LangSmith.

### [Campus Environmental Digital Twin](https://github.com/nhatminh-115/IoT-DigitalTwin-Backend) · Applied ML & Backend

An AI-enabled campus environmental monitoring and forecasting system developed during my UEH internship.

- Built sensor ingestion, normalization, and a deterministic **data-quality gate** for flatlines, outliers, and missing values.
- Developed multivariate **LSTM forecasting**, rolling error diagnostics, and Monte Carlo Dropout uncertainty estimates.
- Integrated an **autoencoder anomaly detector** with feature-level attribution.
- Connected the models to **FastAPI**, a Unity 3D client, Streamlit monitoring, and a Telegram assistant powered by Groq Llama 3.3 70B.

### [Patch-Content Fungibility](https://github.com/nhatminh-115/Patch-Content-Fungibility) · Mechanistic ML Research

A mechanistic investigation of late-layer spatial patch representations in Vision Transformers.

- Studies patch-content replaceability under fixed token positions, sequence length, and model weights.
- Examines feature geometry, token diversity, directional sensitivity, and functional transmission across four pretrained ViT families.
- Includes an operator-aware token-compression benchmark as a bounded application of the mechanistic findings.

## Engineering Toolkit

| Area | Tools and methods |
|---|---|
| **Languages & data** | Python, SQL, Pandas, NumPy |
| **Deep learning** | PyTorch, Transformers, PEFT/LoRA, TRL, SFT, DPO |
| **Computer vision** | YOLO, EfficientNetV2, SigLIP, ByteTrack, OpenCV, ONNX Runtime |
| **LLM systems** | vLLM, AWQ, LangGraph, ChromaDB, RAGAS, LangSmith |
| **Backend & interfaces** | FastAPI, PostgreSQL, Supabase, Streamlit, Unity, Telegram Bot API |
| **MLOps & cloud** | Docker, AWS, Terraform, MLflow, DagsHub, GitHub Actions |

## Education & Credentials

**University of Economics Ho Chi Minh City (UEH)**  
B.Eng. in Robotics & Artificial Intelligence · Expected March 2027  
**GPA: 3.65 / 4.00** &nbsp;·&nbsp; **TOEIC Listening & Reading: 985 / 990**

- Deep Learning Specialization — DeepLearning.AI
- MLOps Specialization — Duke University
- NLP & LLMs — UEH

---

<p align="center">
  <sub>Interested in AI engineering roles across computer vision, LLM systems, and applied ML.</sub>
  <br />
  <sub><a href="https://www.linkedin.com/in/nnminh115/">LinkedIn</a> · <a href="mailto:nhatminhvcst115@gmail.com">Email</a></sub>
</p>
