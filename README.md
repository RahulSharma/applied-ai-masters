# 🗺️ APPLIED AI MASTER'S: 12-MONTH RESOURCE & TOOL MAP

This document serves as the exhaustive tracking layer for all textbook chapters, video series, software engineering toolkits, and interactive environments mapped directly to each Spoke repository.

---

## 🟩 PHASE 1: DEEP FOUNDATIONAL ENGINEERING (MONTHS 1–3)
**Objective:** Build low-level programmatic data structures and core mathematical optimization components from scratch.

### 🟩 Month 1: DSA & Storage Foundations
* **Target Spoke Repository:** `vector-index-engine`
* **Core Tool Stack:** Python 3.11+, `struct`, `pickle`, `unittest`, `pytest`.
* **Primary Learning Resources:**
  * **Certification Course:** *Harvard CS50P (Introduction to Programming with Python)* — Complete Weeks 0 through 5.
  * **Core Documentation/Readings:** Python `struct` module library layout guidelines & RealPython's guide *"Reading and Writing Binary Data in Python"*.
* **System Engineering Target:** Complete `src/storage_core.py` and `src/engine.py` using fixed-width contiguous binary payloads and a streaming min-heap architecture.

### 🟩 Month 2: Linear Algebra & Matrix Computing
* **Target Spoke Repository:** `scratch-neural-layer`
* **Core Tool Stack:** `NumPy` (C-implemented underlying arrays), `SciPy`, `Matplotlib`.
* **Primary Learning Resources:**
  * **Certification Course:** *Mathematics for Machine Learning: Linear Algebra* (Imperial College London via Coursera) — Skip entry-level definitions; focus on matrix transformations and Singular Value Decomposition (SVD).
  * **Visual Series:** 3Blue1Brown's YouTube Series: *Essence of Linear Algebra* — Focus on Dot Products, Change of Basis, and Eigenvalues.
* **System Engineering Target:** Write `src/matrix_ops.py` to evaluate forward-propagation matrices ($Y = WX + B$) using pure NumPy dot products without standard deep learning wrappers.

### 🟩 Month 3: Optimization Dynamics
* **Target Spoke Repository:** `sgd-optimization-engine`
* **Core Tool Stack:** Google `JAX` (Functional API transformations: `jax.grad`, `jax.jit`), `NumPy`.
* **Primary Learning Resources:**
  * **Certification Course:** *Mathematics for Machine Learning: Multivariate Calculus* (Imperial College London via Coursera) — Focus on Jacobians, Hessians, and Chain Rule paths.
  * **Conceptual Videos:** StatQuest with Josh Starmer (YouTube): *Gradient Descent, Step-by-Step* and *Backpropagation Main Ideas*.
  * **Documentation:** *JAX Quickstart Guide* official technical manuals.
* **System Engineering Target:** Write `src/gradient_descent.py` to execute iterative multivariate parameter updates, minimizing Mean Squared Error (MSE) dynamically.

---

## 🟨 PHASE 2: CORE MACHINE LEARNING & NEURAL NETWORKS (MONTHS 4–6)
**Objective:** Handle tabular distributions, class imbalances, ensemble configurations, and multi-channel image tensors.

### 🟨 Month 4: Classical Machine Learning & Explainability
* **Target Spoke Repository:** `b2b-churn-optimizer`
* **Core Tool Stack:** `Scikit-Learn`, `XGBoost`, `LightGBM`, `SHAP`, `MLflow`.
* **Primary Learning Resources:**
  * **Certification Course:** *Machine Learning Specialization - Course 1 & 2* (Stanford/DeepLearning.AI via Coursera) by Andrew Ng.
  * **Core Documentation/Readings:** *SHAP Official Documentation Tutorials* (focusing specifically on tree ensemble configurations via `TreeExplainer`).
  * **Conceptual Videos:** StatQuest with Josh Starmer (YouTube): *XGBoost Series* (Parts 1 to 4).
* **System Engineering Target:** Build `src/pipeline.py` to ingest messy tabular features, balance classes, execute tree metrics, track parameters with local MLflow instances, and output SHAP global importances.

### 🟨 Months 5-6: Deep Learning & Computer Vision
* **Target Spoke Repository:** `medical-vision-cnn`
* **Core Tool Stack:** `PyTorch` (Tensors, Hooks, Optimization paths), `TorchVision`, `TensorBoard`, `Hugging Face Accelerate`.
* **Primary Learning Resources:**
  * **Certification Course:** *Deep Learning Specialization - Course 1 & 4* (DeepLearning.AI via Coursera) — Focus on deep grid adjustments and CNN structures.
  * **Code Implementation Series:** Andrej Karpathy's YouTube Course: *Neural Networks: Zero to Hero* — Focus explicitly on *Building Micrograd* and *Building Makemore* channels.
* **System Engineering Target:** Build `src/train.py` to execute asynchronous data loaders, compute backpropagation over complex image matrices, handle custom evaluation states, and track metrics inside `TensorBoard`.

---

## 🟦 PHASE 3: GENERATIVE AI, LLMs & BIG DATA LAYERS (MONTHS 7–9)
**Objective:** Scale architecture to process massive streaming inputs and orchestrate multi-step context retrieval networks.

### 🟦 Months 7-8: GenAI Foundations, Advanced RAG & Agentic Patterns
* **Target Spoke Repository:** `hybrid-rag-knowledge-graph`
* **Core Tool Stack:** Hugging Face `Transformers`, `Qdrant` or `Milvus`, `LangGraph`, `vLLM` inference engine, `Ollama`.
* **Primary Learning Resources:**
  * **Certification Course:** *Generative AI with Large Language Models* (AWS & DeepLearning.AI via Coursera) — Master scaling parameters, transformer loops, PEFT/LoRA matrix updates, and quantization types (INT8/NF4).
  * **Specialized Short Courses:** DeepLearning.AI: *AI Agents in LangGraph* & *Vector Databases: From Embeddings to Applications*.
  * **Research Paper Literature:** *Attention Is All You Need* (Vaswani et al.) — Core evaluation of Section 1 through 5.
* **System Engineering Target:** Write `src/orchestration.py` to instantiate semantic document parsers, serve local open-weight instances via vLLM, manage indices in Qdrant, and drive state machines via LangGraph.

### 🟦 Month 9: Industrial Scale Big Data Engineering
* **Target Spoke Repository:** `stream-logging-spark-fabric`
* **Core Tool Stack:** `PySpark` (Spark Dataframe and SQL engines), `Delta Lake` core APIs, `Apache Kafka` distributed logs.
* **Primary Learning Resources:**
  * **Certification Pathway:** *Databricks Certified Associate Developer for Apache Spark* self-guided study roadmap (via Databricks Academy or DataCamp).
  * **Architectural Guides:** *Delta Lake Architecture Guide (delta.io)* — Focus on handling ACID mutations on object stores and time-travel querying.
* **System Engineering Target:** Build `src/spark_stream.py` to capture streaming data points from Kafka topics, apply multi-worker windowing matrices via PySpark, and write transaction-safe entries directly into Delta Lake partitions.

---

## 🟪 PHASE 4: CLOUD MLOPS & AUTONOMOUS SYSTEM ARCHITECTURE (MONTHS 10–12)
**Objective:** Package, automate, and safely coordinate production-scale AI ecosystems inside containerized cloud instances.

### 🟪 Months 10-11: Enterprise MLOps Engineering
* **Target Spoke Repository:** `serverless-mlops-pipeline`
* **Core Tool Stack:** `FastAPI` (Async routes), `Docker`, `GitHub Actions` CI/CD pipelines, `AWS SageMaker`, `Prometheus`, `Grafana`.
* **Primary Learning Resources:**
  * **Certification Guide:** *AWS Certified Machine Learning – Specialty* (via Udemy or AWS Skill Builder) — Deep study of automated model hosting configurations.
  * **Technical User Manuals:** *FastAPI Official User Guide* (asynchronous workers) and Nigel Poulton's manual *Docker Deep Dive*.
* **System Engineering Target:** Build `src/app.py` inside a multi-stage Dockerfile configuration, script GitHub Actions automation setups, configure serverless endpoints on AWS, and monitor real-time latency anomalies ($p95, p99$).

### 🟪 Month 12: Master Capstone Project
* **Target Spoke Repository:** `autonomous-analyst-factory`
* **Core Tool Stack:** Complete Stack Integration (`PyTorch` + `vLLM` + `Qdrant` + `LangGraph` + `Docker` + `AWS`).
* **Primary Learning Resources:**
  * **Project Framework:** Codebase synthesis of Spokes 1 through 8. Focus on system trace isolation, telemetry logging, and asynchronous task validation.
* **System Engineering Target:** Build `src/main.py` to orchestrate multi-agent workflows executing deep business analysis tasks, accessing custom binary vector indexes and handling memory footprint metrics natively.

---

## 📊 CORE SKILLS & IMPLEMENTATION MATRIX

| Math & Core Pillar | Target Tool Stack / Engineering Target | Strategic Big Tech Competency |
| :--- | :--- | :--- |
| **Linear Algebra** (The Language of Tensors) | `NumPy`, `SciPy`, Custom C++/Rust Inference Kernels, Eigen/BLAS/LAPACK | Essential for understanding multi-dimensional layer transformations, matrix decomposition (SVD/Eigenvalues), and driving sub-millisecond tensor inference speeds. |
| **Multivariate Calculus** (The Language of Optimization) | `JAX` Automatic Differentiation (`jax.grad`, `jax.jit`), Custom Loss Functions | Required to design custom objective functions, optimize gradient flow, and debug deep neural network backpropagation strings. |
| **Probability & Statistics** (The Language of Uncertainty) | Anomaly Detection Models, `MLflow` Metric Logging, Feature Drift Tracking | Crucial for data-driven debugging, validating inference models under production exceptions, and optimizing LLM sampling boundaries. |
| **Spatial DSA** (High-Throughput Handling) | Streaming Heap Seeks (`heapq`), Memory-Contiguous Byte Mapping (`struct`), HNSW Graphing | Eliminates standard linear search limits ($\mathcal{O}(N)$), maximizing execution performance and cache-locality across millions of embeddings. |
