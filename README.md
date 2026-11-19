# Hi, I'm Minh

**AI Engineer | Robotics & AI, UEH**

Applied AI projects in computer vision, LLM serving, time-series modeling, and IoT, with a focus on inference optimization, evaluation, and deployable backend systems.

---

## Featured Projects

### [SentinelVision](https://github.com/nhatminh-115/SentinelVision-Showcase)

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


### [Campus Environmental Digital Twin](https://github.com/nhatminh-115/IoT-DigitalTwin-Backend)

*Graduation internship project at UEH Campus V, developing an AI-enabled environmental monitoring and forecasting system.*

* **Telemetry pipeline:** Built a resilient ingestion and normalization pipeline that transforms device-level sensor readings into a multivariate time-series dataset, with timestamp parsing, schema normalization, and retry-aware fetching.
* **Data quality:** Implemented a deterministic Data Quality Gate with sensor flatline detection, statistical outlier filtering, and missing-value interpolation before downstream modeling.
* **Forecasting and evaluation:** Developed a first-order-differenced multivariate LSTM for next-step prediction, supported by historical evaluation, rolling MAE/RMSE diagnostics, and Monte Carlo Dropout-based uncertainty estimates.
* **Anomaly detection:** Integrated an autoencoder-based detector using reconstruction-error scoring and feature-level attribution to identify channels contributing most to anomalous readings.
* **Backend and Digital Twin integration:** Exposed FastAPI endpoints for sensor readings and predictions; connected a Unity 3D client and built a Streamlit dashboard for forecast and model-health monitoring.
* **AI-assisted operations:** Built a Telegram assistant powered by Groq Llama 3.3 70B, with intent-based sensor-context routing and semantic caching for repeated operational queries.
* **Deployment:** Containerized the backend with Docker and automated deployment synchronization through GitHub Actions.
---

## Tech Stack

* **LLM and fine-tuning:** `PyTorch` `Transformers` `PEFT/LoRA` `TRL` `SFT` `DPO` `LangGraph` `ChromaDB` `RAGAS` `Groq`
* **Serving and optimization:** `vLLM` `AWQ` `ONNX Runtime` `FP32` `FP16`
* **Computer vision:** `YOLO` `EfficientNetV2` `SigLIP` `ByteTrack` `OpenCV` `WBF`
* **Time-series and anomaly detection:** `LSTM` `Monte Carlo Dropout` `Autoencoder` `Rolling MAE/RMSE`
* **MLOps and cloud:** `Docker` `Terraform` `AWS EC2` `AWS S3` `MLflow` `DagsHub` `GitHub Actions`
* **Backend and data:** `FastAPI` `Streamlit` `Unity 3D` `Telegram Bot API` `PostgreSQL` `Supabase` `Python`

---

## Certifications

* **Deep Learning Specialization** — DeepLearning.AI
* **MLOps Specialization** — Duke University

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/nnminh115/)
