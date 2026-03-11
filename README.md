# Arunark Singh

**Electrical Engineer · UBC** — building intelligent systems at the intersection of robotics, machine learning, and microsystem design.

I work across the full stack of autonomous systems: from low-level embedded firmware and MEMS sensor architectures, to perception pipelines and deep learning models. I care about systems that work in the real world — reliable, efficient, and well-engineered end to end.

Currently seeking **full-time or internship roles** in robotics, ML engineering, or embedded/perception systems.

📍 Vancouver, BC &nbsp;|&nbsp; 📧 [arunarksingh@gmail.com](mailto:arunarksingh@gmail.com) &nbsp;|&nbsp; 🔗 [LinkedIn](https://linkedin.com/in/arunark-singh)

---

## 🛠️ Technical Skills

| Domain | Tools & Technologies |
|---|---|
| **Languages** | Python, C++ |
| **Robotics** | ROS / ROS2, PX4, Gazebo, SLAM, VINS-Fusion, OpenCV |
| **ML / DL** | PyTorch, HuggingFace Transformers, scikit-learn, XGBoost, Weights & Biases |
| **Embedded** | STM32, Raspberry Pi, FPGA, PCB Design |
| **MEMS & CAD** | COMSOL Multiphysics, CleWin, MATLAB |
| **Deployment** | FastAPI, Git |

---

## 🚀 Selected Projects

### Autonomous Systems & Robotics

**[Autonomous Indoor Drone Navigation for 3D Reconstruction](https://github.com/ArunarkSingh/Autonomous_Inspection_Drone_ICON)**  
Full autonomous navigation stack for indoor 3D reconstruction — integrating PX4 flight control, VINS-Fusion for visual-inertial odometry, FUEL for exploration planning, and a RealSense depth camera. Handles real-time state estimation, motion planning, and map building in GPS-denied environments.  
`ROS` `PX4` `VINS-Fusion` `C++` `Python` `RealSense`

---

### Deep Learning & Generative Models

**[Conditional PixelCNN++ — Generation & Zero-Shot Classification](https://github.com/ArunarkSingh/Conditional_PixelCNN-Plus)**  
Extended PixelCNN++ with early fusion and FiLM-based conditioning to support class-conditional image generation and likelihood-based zero-shot classification. Best model: **FID 28**, **74% validation accuracy**.  
`PyTorch` `PixelCNN++` `FiLM Conditioning` `Weights & Biases`

---

### Machine Learning Engineering

**[Paper Navigator — Semantic Search over ML ArXiv Papers](https://github.com/ArunarkSingh/paper-navigator)**
Two-stage retrieval system over ~15k chunked ArXiv abstracts: dense ANN search via FAISS HNSW followed by cross-encoder reranking. Papers are split into overlapping 220-word chunks with title/abstract context prepended for retrieval quality. Benchmarked at **~174ms p50 (dense)** and **~329ms p50 (reranked)**. Refactored from a research notebook into a modular, locally-runnable CLI pipeline.
`Python` `FAISS` `SentenceTransformers` `HuggingFace` `Cross-Encoder Reranking`

**[Customer Churn Prediction — Business-Aware ML Pipeline](https://github.com/ArunarkSingh/Customer-Churn-Prediction-Business-ML)**  
End-to-end churn prediction pipeline using Logistic Regression and XGBoost, with decision threshold optimization for expected business retention value under class imbalance. Includes SHAP explainability and FastAPI deployment.  
`Python` `XGBoost` `SHAP` `FastAPI` `scikit-learn`

**[Fake News Detection with RoBERTa (LIAR Dataset)](https://github.com/ArunarkSingh/Fake-News-Detection-Roberta)**  
Fine-tuned RoBERTa-base on ~12k political statements for fact-checking. Achieved **60.5% test accuracy (macro-F1: 0.587)** on binary classification and **29.4%** on the full 6-class task. Deployed as a FastAPI inference service with full evaluation suite (ROC/PR curves, confusion matrices, per-class F1).  
`PyTorch` `HuggingFace Transformers` `RoBERTa` `FastAPI` `scikit-learn`

**[Credit Card Fraud Detection — Imbalanced Classification](https://github.com/ArunarkSingh/CreditCard_Fraud_Detection_Imbalanced_ML)**  
Fraud detection pipeline under extreme class imbalance (~0.17% positive rate), optimized for recall using precision-recall analysis and threshold tuning rather than default accuracy metrics.  
`Python` `scikit-learn` `PR/ROC Analysis`

---

## 🎓 Education

**B.ASc. Electrical Engineering** — University of British Columbia (UBC)  
Focus: Robotics, MEMS, Machine Learning

---

*Open to robotics engineering, ML engineering, and embedded/perception roles. Feel free to reach out or explore the repos above.*
