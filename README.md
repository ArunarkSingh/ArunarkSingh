# Arunark Singh

**Machine Learning Engineer & Data Scientist** - building end-to-end machine learning systems from data pipelines to deployed models.

I work across the ML stack: foundation model fine-tuning, semantic search and RAG systems, tabular ML, and data analysis pipelines. I care about systems that are well-engineered, reproducible, and grounded in real data.

Incoming **UBC Master of Data Science** student (September 2026). Currently seeking internship or new grad roles in ML engineering and data science.

Vancouver, BC | [arunarksingh@gmail.com](mailto:arunarksingh@gmail.com) | [LinkedIn](https://linkedin.com/in/arunark-singh)

---

## Technical Skills

| Domain | Tools & Technologies |
|---|---|
| **Languages** | Python, SQL, C/C++, Bash, R |
| **ML / DL** | PyTorch, HuggingFace Transformers, scikit-learn, XGBoost, LLM Fine-tuning, Transformer Architectures |
| **Data & Pipelines** | pandas, NumPy, Feature Engineering, Reproducible Pipelines, Structured & Unstructured Data |
| **Search & Retrieval** | FAISS, Semantic Search, RAG, Vector Embeddings, Cross-Encoder Reranking |
| **MLOps & Cloud** | Azure ML, AWS, Docker, FastAPI, Git, Weights & Biases, CUDA, Mixed-Precision Training |

---

## Projects

### Machine Learning & Data Science

**[Vancouver Rental Market Analysis](https://github.com/ArunarkSingh/rental-market-analysis-vancouver)**  
Scraped 342 live Craigslist listings across Metro Vancouver, joined with SkyTrain station coordinates, and built an end-to-end analysis pipeline to answer: which neighbourhoods are underpriced, does transit proximity affect rent, and what features drive price most? Key finding: neighbourhood accounts for more price variance than SkyTrain proximity. Includes GBM model with SHAP explainability, SQL analysis (SQLite), and an interactive Folium map.  
`Python` `pandas` `scikit-learn` `SHAP` `SQLite` `Folium` `BeautifulSoup`

**[Neural Research Paper Navigator - Hybrid Retrieval and RAG](https://github.com/ArunarkSingh/neural-paper-navigator-rag)**  
Hybrid neural retrieval and RAG system over ~15k chunked ArXiv ML papers. Dense ANN search via FAISS HNSW with BGE embeddings, fused with BM25 sparse retrieval and cross-encoder reranking. Achieved ~12ms p50 dense retrieval latency and ~163ms p50 with reranking. Refactored from research prototype into a modular CLI pipeline with RAGAS-style evaluation metrics.  
`Python` `FAISS` `SentenceTransformers` `HuggingFace` `Cross-Encoder Reranking` `RAG`

**[Customer Churn Prediction - Business-Aware ML Pipeline](https://github.com/ArunarkSingh/Customer-Churn-Prediction-Business-ML)**  
End-to-end churn prediction pipeline reframed as a cost-sensitive retention optimization rather than accuracy maximization. Decision threshold tuned on expected business retention value under class imbalance. Includes SHAP explainability and FastAPI deployment.  
`Python` `XGBoost` `SHAP` `FastAPI` `scikit-learn`

**[Fake News Detection with RoBERTa (LIAR Dataset)](https://github.com/ArunarkSingh/Fake-News-Detection-Roberta)**  
Fine-tuned RoBERTa-base on ~12k political statements for 6-class fact-checking classification. Achieved 60.5% test accuracy (macro-F1: 0.587). Deployed as a FastAPI inference service with full evaluation suite (ROC/PR curves, confusion matrices, per-class F1).  
`PyTorch` `HuggingFace Transformers` `RoBERTa` `FastAPI` `scikit-learn`

**[Credit Card Fraud Detection - Imbalanced Classification](https://github.com/ArunarkSingh/CreditCard_Fraud_Detection_Imbalanced_ML)**  
Fraud detection under extreme class imbalance (~0.17% positive rate). Optimized for recall via precision-recall analysis and validation-based threshold tuning. Achieved recall ~87% and AUC = 0.966.  
`Python` `scikit-learn` `PR/ROC Analysis`

---

### Deep Learning

**[Conditional PixelCNN++ - Generation & Zero-Shot Classification](https://github.com/ArunarkSingh/Conditional_PixelCNN-Plus)**  
Extended PixelCNN++ with early fusion and FiLM-based conditioning for class-conditional image generation and likelihood-based zero-shot classification. Best model: FID 28, 74% validation accuracy.  
`PyTorch` `PixelCNN++` `FiLM Conditioning` `Weights & Biases`

---

### Robotics  

**[Autonomous Indoor Drone Navigation for 3D Reconstruction](https://github.com/ArunarkSingh/Autonomous_Inspection_Drone_ICON)**  
Full autonomous navigation stack integrating PX4 flight control, VINS-Fusion for visual-inertial odometry, FUEL for exploration planning, and a RealSense depth camera in GPS-denied environments.  
`ROS` `PX4` `VINS-Fusion` `C++` `Python`

---

## Education

**M.Sc. Data Science** - University of British Columbia (UBC) - Start September 2026  
**B.ASc. Electrical Engineering** - University of British Columbia (UBC) - Graduated May 2026

---

*Open to ML engineering and data science internship or new grad roles. Feel free to reach out or explore the repos above.*
