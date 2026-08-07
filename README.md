<div align="center">

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=600&size=24&duration=2800&pause=900&color=6C63FF&center=true&vCenter=true&width=520&lines=Machine+Learning+Engineer;LLM+Fine-Tuning+%26+RAG+Systems;Retrieval%2C+Generative+Models%2C+Tabular+ML;Incoming+UBC+MDS+2026" alt="Typing SVG" />

# Arunark Singh

**Building end-to-end ML systems — from data pipelines to deployed models.**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/arunark-singh)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:arunarksingh@gmail.com)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/Arunark)
![Location](https://img.shields.io/badge/Vancouver,%20BC-3D3D3D?style=for-the-badge&logo=googlemaps&logoColor=white)

</div>

---

I work across the ML stack: foundation model fine-tuning, semantic search and RAG, generative modeling, and tabular ML with real business constraints. I care about systems that are **reproducible**, **honestly evaluated**, and **grounded in real data** — not benchmark theater.

```yaml
name:      Arunark Singh
education: B.ASc. Electrical Engineering, UBC (2026) → M.Sc. Data Science, UBC (Sep 2026)
focus:     [LLM fine-tuning, retrieval systems, generative models, applied ML]
building:  judge-free eval harnesses for tool-calling LLMs
seeking:   ML Engineer / Data Scientist — internship & new grad
```

---

# Projects

Grouped by domain. Each cluster is a different part of the stack I've worked in.

<div align="center">

[![LLM](https://img.shields.io/badge/①%20LLM%20Systems%20%26%20Retrieval-6C63FF?style=for-the-badge)](#-llm-systems--retrieval)
[![DL](https://img.shields.io/badge/②%20Deep%20Learning%20%26%20Generative-1f6feb?style=for-the-badge)](#-deep-learning--generative-modeling)
[![Applied](https://img.shields.io/badge/③%20Applied%20ML%20%26%20Data%20Science-2ea043?style=for-the-badge)](#-applied-ml--data-science)
[![Robotics](https://img.shields.io/badge/④%20Robotics%20%26%20Autonomy-d29922?style=for-the-badge)](#-robotics--autonomous-systems)

</div>

---

## ① LLM Systems & Retrieval

*Decoder-only fine-tuning, hybrid retrieval, and judge-free evaluation of model behaviour.*

> ### [Function-Calling LoRA Fine-Tuning](https://github.com/ArunarkSingh/qwen-function-calling-lora) &nbsp;·&nbsp; ![](https://img.shields.io/badge/31%25%20→%2079%25%20exact%20match-6C63FF?style=flat-square)
>
> Fine-tuned **Qwen2.5-1.5B** with 4-bit QLoRA to reliably emit structured tool calls. Trained on xLAM with tool schemas in the system prompt and completion-only loss, so the model *produces* calls instead of echoing schemas.
>
> Evaluated with a **judge-free** metric — strict BFCL-style AST match on function name *and* parsed JSON arguments. Error analysis shows format (99% JSON validity) and tool selection (98% name accuracy) fully solved; residual misses are argument-level. Adapter published to the HF Hub; runs end-to-end on free-tier Colab.
>
> `PyTorch` `Transformers` `PEFT` `QLoRA` `bitsandbytes` `TRL`

<table>
<tr>
<td width="50%" valign="top">

### [Neural Paper Navigator](https://github.com/ArunarkSingh/neural-paper-navigator-rag)
Hybrid retrieval + RAG over ~15k chunked ArXiv ML papers. FAISS HNSW dense search with BGE embeddings, fused with BM25 and cross-encoder reranking. Refactored from research prototype into a modular CLI pipeline with RAGAS-style eval.

![](https://img.shields.io/badge/12ms%20p50%20dense-6C63FF?style=flat-square) ![](https://img.shields.io/badge/163ms%20w%2F%20rerank-6C63FF?style=flat-square)

`FAISS` `SentenceTransformers` `BM25` `Cross-Encoder` `RAG`

</td>
<td width="50%" valign="top">

### Agent Evaluation Harness &nbsp;![](https://img.shields.io/badge/in%20progress-8b949e?style=flat-square)
τ²-bench-style evaluation of tool-using agents — measuring task completion and tool-selection behaviour rather than surface text quality. Includes a retrieval ablation to isolate what actually drives agent success.

![](https://img.shields.io/badge/agent%20eval-8b949e?style=flat-square) ![](https://img.shields.io/badge/tool%20use-8b949e?style=flat-square)

`Python` `LLM Agents` `Ablation Studies`

</td>
</tr>
</table>

---

## ② Deep Learning & Generative Modeling

*Paper-to-implementation work: architecture modification, conditioning mechanisms, and transformer fine-tuning.*

<table>
<tr>
<td width="50%" valign="top">

### [Conditional PixelCNN++](https://github.com/ArunarkSingh/Conditional_PixelCNN-Plus)
Extended PixelCNN++ with early fusion and FiLM-based conditioning for class-conditional generation and likelihood-based zero-shot classification.

![](https://img.shields.io/badge/FID%2028-1f6feb?style=flat-square) ![](https://img.shields.io/badge/74%25%20val%20acc-1f6feb?style=flat-square)

`PyTorch` `PixelCNN++` `FiLM Conditioning` `Weights & Biases`

</td>
<td width="50%" valign="top">

### [Fake News Detection — RoBERTa](https://github.com/ArunarkSingh/Fake-News-Detection-Roberta)
Fine-tuned RoBERTa-base on ~12k LIAR political statements for 6-class fact-checking. Served via FastAPI with a full evaluation suite: ROC/PR curves, confusion matrices, per-class F1.

![](https://img.shields.io/badge/60.5%25%20accuracy-1f6feb?style=flat-square) ![](https://img.shields.io/badge/macro--F1%200.587-1f6feb?style=flat-square)

`PyTorch` `Transformers` `RoBERTa` `FastAPI`

</td>
</tr>
</table>

---

## ③ Applied ML & Data Science

*Real data, real constraints — cost-sensitive decisions, class imbalance, and explainability that survives stakeholder questions.*

<table>
<tr>
<td width="50%" valign="top">

### [Vancouver Rental Market Analysis](https://github.com/ArunarkSingh/rental-market-analysis-vancouver)
Scraped 342 live Craigslist listings, joined to SkyTrain station coordinates, and asked what actually drives rent. Finding: **neighbourhood explains more price variance than transit proximity.** GBM + SHAP, SQL analysis, interactive Folium map.

![](https://img.shields.io/badge/342%20listings-2ea043?style=flat-square) ![](https://img.shields.io/badge/SHAP%20%2B%20SQL%20%2B%20Folium-2ea043?style=flat-square)

`pandas` `scikit-learn` `SHAP` `SQLite` `Folium` `BeautifulSoup`

</td>
<td width="50%" valign="top">

### [Customer Churn Pipeline](https://github.com/ArunarkSingh/Customer-Churn-Prediction-Business-ML)
Reframed churn as **cost-sensitive retention optimization**, not accuracy maximization. Decision threshold tuned on expected business retention value under class imbalance. SHAP explainability + FastAPI deployment.

![](https://img.shields.io/badge/business--value%20threshold-2ea043?style=flat-square) ![](https://img.shields.io/badge/SHAP%20%2B%20FastAPI-2ea043?style=flat-square)

`XGBoost` `SHAP` `FastAPI` `scikit-learn`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [Credit Card Fraud Detection](https://github.com/ArunarkSingh/CreditCard_Fraud_Detection_Imbalanced_ML)
Detection under extreme class imbalance (~0.17% positive rate). Optimized for recall via precision-recall analysis and validation-based threshold tuning rather than raw accuracy.

![](https://img.shields.io/badge/recall%20~87%25-2ea043?style=flat-square) ![](https://img.shields.io/badge/AUC%200.966-2ea043?style=flat-square)

`Python` `scikit-learn` `PR/ROC Analysis`

</td>
<td width="50%" valign="top">

### Causal Inference — Interrupted Time Series &nbsp;![](https://img.shields.io/badge/in%20progress-8b949e?style=flat-square)
Quasi-experimental evaluation of a policy intervention using interrupted time series, with HAC/Newey-West standard errors to handle autocorrelation in the residuals.

![](https://img.shields.io/badge/causal%20inference-8b949e?style=flat-square) ![](https://img.shields.io/badge/statistical%20rigor-8b949e?style=flat-square)

`Python` `statsmodels` `Time Series`

</td>
</tr>
</table>

---

## ④ Robotics & Autonomous Systems

*Where I came from — embedded systems, sensor fusion, and perception under hard real-time constraints.*

> ### [Autonomous Indoor Drone Navigation for 3D Reconstruction](https://github.com/ArunarkSingh/Autonomous_Inspection_Drone_ICON)
>
> Full autonomous navigation stack for GPS-denied environments: **PX4** flight control, **VINS-Fusion** visual-inertial odometry, **FUEL** exploration planning, and a RealSense depth camera for onboard reconstruction. Capstone project bridging my electrical engineering background into perception and state estimation.
>
> `ROS` `PX4` `VINS-Fusion` `C++` `Python` `RealSense`

---

## Tech Stack

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**ML / Deep Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=flat-square)
![PEFT](https://img.shields.io/badge/PEFT%20%2F%20QLoRA-6C63FF?style=flat-square)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)

**Retrieval & Data**

![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logo=meta&logoColor=white)
![BM25](https://img.shields.io/badge/BM25-555555?style=flat-square)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)

**MLOps & Infra**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Azure](https://img.shields.io/badge/Azure%20ML-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![W&B](https://img.shields.io/badge/Weights%20%26%20Biases-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Robotics**

![ROS](https://img.shields.io/badge/ROS-22314E?style=flat-square&logo=ros&logoColor=white)
![PX4](https://img.shields.io/badge/PX4-1B1B1B?style=flat-square)
![RealSense](https://img.shields.io/badge/Intel%20RealSense-0071C5?style=flat-square&logo=intel&logoColor=white)

</div>

<details>
<summary><b>Full breakdown by domain</b></summary>

<br>

| Domain | Tools & Techniques |
|---|---|
| **ML / DL** | LLM fine-tuning (LoRA/QLoRA), transformer architectures, HistGradientBoosting, logistic regression, mixed-precision training, multi-GPU scaling |
| **Data & Pipelines** | Feature engineering, reproducible pipelines, structured & unstructured data, class imbalance handling, threshold optimization |
| **SQL** | Aggregations, window functions, joins, CASE expressions, query optimization |
| **Search & Retrieval** | FAISS HNSW, dense & sparse retrieval, vector embeddings, cross-encoder reranking, RAG evaluation (RAGAS-style) |
| **Evaluation** | SHAP, PR/ROC analysis, confusion matrices, per-class F1, ablation studies, AST-match / judge-free metrics |
| **Statistics** | Interrupted time series, HAC/Newey-West standard errors, quasi-experimental design |
| **Visualization** | Matplotlib, Seaborn, Folium, TensorBoard |

</details>

---

## GitHub Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=ArunarkSingh&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&title_color=6C63FF&icon_color=6C63FF&theme=tokyonight" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ArunarkSingh&layout=compact&langs_count=8&hide_border=true&title_color=6C63FF&theme=tokyonight" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=ArunarkSingh&bg_color=1a1b27&color=6C63FF&line=6C63FF&point=ffffff&area=true&hide_border=true" width="98%" />

</div>

---

<div align="center">

**Open to ML engineering and data science internship & new grad roles.**

Feel free to reach out — or just dig through the repos above.

</div>
