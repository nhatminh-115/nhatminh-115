# Hi, I'm Minh

**AI Engineer | Robotics & AI, UEH**

Applied AI projects in computer vision, LLM serving, and IoT, with a focus on inference optimization, evaluation, and deployable backend systems.

---

## Featured Projects

### [SentinelVision](https://github.com/nhatminh-115/SentinelVision)

*Real-time PPE compliance monitoring with computer vision, automated evaluation, and regulation-grounded reporting.*

* **Detection and tracking:** YOLO11s + YOLO26l ensemble with Weighted Boxes Fusion, ByteTrack, and Box EMA for stable multi-person tracking.
* **PPE classification:** EfficientNetV2-B0 ONNX FP32 achieves **7.46 ms CPU latency** versus ~45 ms in PyTorch (about **6× faster**, F1 = 0.92) for small boxes. SigLIP SO400M ONNX FP16 handles larger boxes with **3.2× GPU speedup**, **2× smaller model size**, and 0.999997 cosine similarity to the PyTorch output.
* **State management:** Hysteresis FSM and classify-lock logic suppress repeated alerts and avoid redundant GPU inference for stable tracks.
* **Evaluation feedback loop:** Human-confirmed labels are versioned and exported to S3. EC2 Spot retraining is triggered only when the 7-day rolling human disagreement rate exceeds 0.25 and at least 100 confirmed labels are available.
* **Reporting:** LangGraph pipeline with ChromaDB RAG over Vietnam Circular 25/2022/TT-BLDTBXH generates daily compliance reports with regulation citations.
* **Infrastructure:** Docker, Terraform on AWS, GitHub Actions CI/CD, Supabase, and MLflow/DagsHub experiment tracking.

### [ReframeBot](https://github.com/nhatminh-115/ReframeBot)

*CBT-oriented chatbot for academic stress, focused on efficient local LLM serving, guardrail routing, and RAG evaluation.*

* **Fine-tuning and compression:** Fine-tuned Llama 3.1 8B with SFT + DPO through PEFT/LoRA, then applied AWQ 4-bit quantization to reduce serving VRAM to approximately **5.4 GB**.
* **Serving:** Dockerized vLLM and FastAPI stack with an OpenAI-compatible API, PagedAttention, continuous batching, and SSE streaming. On an RTX 5070 8 GB GPU, measured p50 latency of **2.6 s**, p50 TTFT of **1.11 s**, and approximately **39 tokens/s**.
* **Guardrail routing:** DistilBERT 3-class classifier for CBT, crisis, and out-of-scope routing, backed by regex and semantic crisis signals. Achieved **98.3% accuracy on a 60-example out-of-domain hard evaluation set** using a `P(TASK_2) >= 0.10` threshold selected to prioritize crisis recall.
* **RAG observability:** LangSmith tracing and RAGAS evaluation over a ChromaDB CBT knowledge base. Topic-aware chunking and retrieval tuning achieved faithfulness of **0.7388** and context precision/recall of **0.8125**.

### [GreenCalyx AI](https://github.com/nhatminh-115/GreenCalyx_AI)

*Logistics ESG scoring tool developed for the CAIEC Competition.*

* **Document pipeline:** LangGraph workflow parses five trade-document types (CI, PL, BL/AWB, TDS, and PPWR) using Groq Llama 4 Scout vision.
* **Emissions estimation:** Calculates CO2e using GLEC Framework v3.2 and ISO 14083-aligned logic, with sea-route estimation through `searoute-py`.
* **Output:** Produces a 0–100 ESG score with GREEN, YELLOW, and RED lane classification; stores results in Supabase.

### [Digital Twin: Environment Monitoring](https://github.com/nhatminh-115/IoT-DigitalTwin-Backend)

*Graduation internship at UEH Campus V, Jun 2025 – Jun 2026.*

* LSTM one-step forecasting and autoencoder-based anomaly detection across eight sensor nodes.
* Data-quality pipeline for flatline detection, z-score outlier filtering, and linear interpolation.
* Telegram assistant using Groq Llama 3.3 70B with intent-based context routing.
* Real-time Unity 3D visualization deployed on a VPS.

---

## Tech Stack

* **LLM and fine-tuning:** `PyTorch` `Transformers` `PEFT/LoRA` `TRL` `SFT` `DPO` `LangGraph` `ChromaDB` `RAGAS` `Groq`
* **Serving and optimization:** `vLLM` `AWQ` `ONNX Runtime` `FP32` `FP16`
* **Computer vision:** `YOLO` `EfficientNetV2` `SigLIP` `ByteTrack` `OpenCV` `WBF`
* **MLOps and cloud:** `Docker` `Terraform` `AWS EC2` `AWS S3` `MLflow` `DagsHub` `GitHub Actions`
* **Backend and data:** `FastAPI` `PostgreSQL` `Supabase` `Python` `MQTT`

---

## Certifications

* **Deep Learning Specialization** — DeepLearning.AI
* **MLOps Specialization** — Duke University

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/nnminh115/)
