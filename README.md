<p align="center">
  <img src="assets/minh-profile-banner.svg" alt="Nhat Minh — AI / ML Engineer" width="100%" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/nnminh115/">LinkedIn</a>
  &nbsp;·&nbsp;
  <a href="mailto:nhatminhvcst115@gmail.com">Email</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/nhatminh-115">GitHub</a>
</p>

<p align="center">
  <strong>Ho Chi Minh City, Vietnam</strong> &nbsp;·&nbsp; Robotics &amp; Artificial Intelligence, UEH &nbsp;·&nbsp; Class of 2027
</p>

<p align="center">
  <img src="assets/about-panel.svg" alt="About: I build applied AI systems across computer vision, LLM applications and machine learning, focusing on data quality, evaluation, inference, backend integration and deployment." width="100%" />
</p>

[![SentinelVision: real-time PPE monitoring with YOLO detection, ByteTrack, size-routed classifiers, parallel alerts and a human-confirmed MLOps retraining loop.](assets/work-sentinelvision.svg)](https://github.com/nhatminh-115/SentinelVision)

<details>
  <summary>Technical notes — SentinelVision</summary>

  - **Detection and tracking:** YOLO ensemble, Weighted Boxes Fusion, ByteTrack, and temporal smoothing for multi-person tracking.
  - **Dual-path classification:** EfficientNetV2-B0 ONNX for small person boxes; SigLIP SO400M ONNX FP16 for larger boxes.
  - **Inference optimization:** EfficientNet ONNX reaches **7.46 ms CPU latency** with **F1 = 0.92** on the small-box route; SigLIP ONNX FP16 delivers **3.2× GPU speedup** over its PyTorch FP32 baseline.
  - **Human-in-the-loop MLOps:** versioned human-confirmed labels, disagreement monitoring, gated EC2 Spot retraining, and MLflow/DagsHub artifact tracking.
</details>

[![ReframeBot: local LLM application with Llama 3.1 8B fine-tuning, AWQ quantization, vLLM serving, safety routing and RAGAS evaluation.](assets/work-reframebot.svg)](https://github.com/nhatminh-115/ReframeBot)

<details>
  <summary>Technical notes — ReframeBot</summary>

  - Fine-tuned Llama 3.1 8B with **SFT + DPO**, then applied **AWQ 4-bit quantization**.
  - Served through a Dockerized **vLLM + FastAPI** stack with PagedAttention, continuous batching, and SSE streaming.
  - Added a DistilBERT guardrail router for CBT, crisis, and out-of-scope inputs, with explicit crisis-signal handling.
  - Evaluated retrieval quality with **RAGAS** and traced application behavior with LangSmith.
</details>

[![UEH Campus Digital Twin: sensor telemetry, reliability checks, LSTM forecasting, autoencoder anomaly signals, FastAPI, Unity 3D, Streamlit and Telegram AI assistant.](assets/work-digital-twin.svg)](https://github.com/nhatminh-115/IoT-DigitalTwin-Backend)

<details>
  <summary>Technical notes — UEH Campus Digital Twin</summary>

  - Built sensor ingestion, normalization, and a deterministic **data-quality gate** for flatlines, outliers, and missing values.
  - Developed multivariate **LSTM forecasting**, rolling error diagnostics, and Monte Carlo Dropout uncertainty estimates.
  - Integrated an **autoencoder anomaly detector** with feature-level attribution.
  - Connected the models to **FastAPI**, a Unity 3D client, Streamlit monitoring, and a Telegram assistant powered by Groq Llama 3.3 70B.
</details>

[![Patch-Content Fungibility: mechanistic investigation of late-layer Vision Transformer patch representations and operator-aware token compression.](assets/work-pcf.svg)](https://github.com/nhatminh-115/Patch-Content-Fungibility)

<details>
  <summary>Technical notes — Patch-Content Fungibility</summary>

  - Studies patch-content replaceability under fixed token positions, sequence length, and model weights.
  - Examines feature geometry, token diversity, directional sensitivity, and functional transmission across four pretrained ViT families.
  - Includes an operator-aware token-compression benchmark as a bounded application of the mechanistic findings.
</details>

<p align="center">
  <img src="assets/toolkit-panel.svg" alt="Engineering toolkit: Python, PyTorch, Transformers, Pandas, NumPy, PEFT, YOLO, ONNX, vLLM, AWQ, FastAPI, RAGAS, LangGraph, Docker, AWS, Terraform, PostgreSQL and MLflow." width="100%" />
</p>

<p align="center">
  <img src="assets/education-panel.svg" alt="UEH B.Eng. Robotics and Artificial Intelligence, expected March 2027; GPA 3.65 out of 4.00; TOEIC Listening and Reading 985 out of 990." width="100%" />
</p>

<details>
  <summary>Additional credentials</summary>

  - Deep Learning Specialization — DeepLearning.AI
  - MLOps Specialization — Duke University
  - NLP &amp; LLMs — UEH
</details>

<p align="center">
  <sub>Interested in AI engineering roles across computer vision, LLM systems, and applied ML.</sub>
</p>
