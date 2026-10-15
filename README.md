<h1 align="center">Anas Tber</h1>

<p align="center">
  <b>Final-year Engineering Student · Machine Learning & AI Engineering</b><br/>
  École Centrale de Lyon · Lyon, France
</p>

<p align="center">
  <a href="https://anastber.com"><img src="https://img.shields.io/badge/Website-anastber.com-111827?style=flat-square&logo=googlechrome&logoColor=white" alt="Website"/></a>
  <a href="https://www.linkedin.com/in/anas-tber-99b994222/"><img src="https://img.shields.io/badge/LinkedIn-Anas%20Tber-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:anas.tber@etu.ec-lyon.fr"><img src="https://img.shields.io/badge/Email-anas.tber%40etu.ec--lyon.fr-374151?style=flat-square&logo=maildotru&logoColor=white" alt="Email"/></a>
</p>

<p align="center">
  🔎 <b>Open to a 6-month end-of-studies internship from late March 2027</b><br/>
  ML Engineering · AI Engineering · Applied AI · Software Engineering
</p>

---

### About

Final-year engineering student at École Centrale de Lyon, specialising in data science and machine learning. I care about understanding *why* models work, not just *that* they do, and I'm most interested in the engineering side of AI: taking models from notebook to production, building reliable ML pipelines, and shipping AI features people actually use. 

---

### Experience

**Data Scientist Intern — BNP Paribas CIB** · *Compliance, Anti-Money Laundering*
<sub>Paris · Jan. 2026 – Jul. 2026</sub>

- Delivered a **regulator-approved** network-based AML detection & investigation platform on a **10M+ entity / 40M+ transaction** dataset, from raw ingestion (Polars / PyArrow lazy mode) to compliance dashboards
- Designed the detection layer on engineered graph features: cycle detection (SCC + DFS) to surface money-mule rings, and an **Isolation Forest + SHAP** model ranking suspicious communities with regulator-facing justifications
- Shipped **LLM-powered features** into the Streamlit app: one-click risk summaries of a community graph and a multi-turn investigation chatbot over an account's 3-hop neighbourhood
- Sole owner of the repository: led the refactor (modular architecture, centralised configuration) and wrote the technical documentation for handover to IT

**Tech & Operations Intern — Gentle Mates** · *Professional Esports*
<sub>Paris · Apr. 2025 – Nov. 2025</sub>

- Built an automated social media analytics dashboard combining **computer vision (YOLO)** for sponsor logo detection and NLP / Regex for brand mention tracking
- Trained a YOLO model on a custom-built dataset of sponsor logos
- Built a cross-platform **React Native** app integrating Valorant & Fortnite APIs for real-time player analytics

---

### Selected Projects

#### 🎹 AirKeys — Camera-Based Gesture Instrument
<sub>Applied ML & Evaluation · 2026 – present · <a href="https://github.com/anastber/REPO_NAME">Code</a> · <a href="LIVE_DEMO_URL">Live demo</a></sub>

- Real-time hand gesture recognition running fully in the browser: MediaPipe landmarks, a self-trained classifier and on-the-fly personalisation via a from-scratch k-NN
- **Leakage-safe evaluation** on 12.5k hands from 9k subjects (HaGRID): subject-disjoint splits, deduplication, grouped CV, bootstrap CIs — showed a single-user model's 99.8% accuracy drops to 72% on unseen people, while a multi-subject model reaches 98%
- Now working on open-set rejection and temporal smoothing after live-webcam testing
- Stack: Python, scikit-learn, MediaPipe, Next.js / TypeScript, Tone.js


#### 📚 arXiv Research Radar — RAG over Recent Papers
<sub>RAG Pipeline · 2026 – present · <a href="https://github.com/anastber/REPO_NAME">Code</a></sub>
 
- End-to-end RAG system answering questions over the latest arXiv papers with **per-claim citations**: PDF ingestion, section-aware chunking, Sentence-Transformers + FAISS retrieval, answers grounded only in retrieved sources (prompt-injection guard)
- Served via **FastAPI + Streamlit** with cost controls (per-IP rate limiting, atomic SQLite daily cap, relevance threshold that skips the LLM on off-topic queries)
- Index refreshed weekly by a **GitHub Actions** pipeline; unit and API tests run in CI on every push
- Now building a **measurement-first evaluation framework** on a frozen 437-paper benchmark (Recall@k, MRR, nDCG, LLM-judged faithfulness and citation precision) to drive the next steps — hybrid search, cross-encoder reranking and scaling to 5–10k papers — each validated by ablation

#### Other work

- **Survival Analysis — ENS Data Challenge (QRT):** gradient boosting on censored genomic & clinical data, **0.7745 IPCW C-index**
- **YouTube Sentiment Analyzer:** RoBERTa / BERT (Hugging Face) on comments fetched via the YouTube Data API, with Plotly visualisations

---

### Skills

| | |
|---|---|
| **Machine Learning** | PyTorch · scikit-learn · LightGBM · SHAP · Pandas · Polars · NumPy |
| **LLM & NLP** | RAG (embeddings, FAISS) · LangChain · Transformers · Gemini / Anthropic / OpenAI APIs · Prompt engineering |
| **Computer Vision** | MediaPipe · OpenCV · YOLO |
| **Engineering & Deployment** | FastAPI · Streamlit · GitHub Actions · SQL / PostgreSQL · Git |
| **Software Development** | Python · JavaScript |

<sub>Languages: French (native) · Arabic (native) · English (fluent) · Turkish (intermediate) · Spanish (beginner)</sub>
