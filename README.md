# 🧠 RAG‑GROQ‑Streamlit

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ritwik4m/rag-groq-streamlit/blob/main/Basic_RAG_pipeline.ipynb)

A beginner‑friendly **Retrieval‑Augmented Generation (RAG)** demo using Wikipedia, FAISS, and Hugging Face models — with optional Streamlit integration.

This project demonstrates how to enhance a language model’s responses by retrieving relevant external knowledge before generating answers, reducing hallucinations and providing grounded, up‑to‑date context.

---

## 🚀 What This Does

This notebook and pipeline:

1. Fetches topic content from Wikipedia
2. Splits text into overlapping chunks
3. Generates dense embeddings for each chunk
4. Stores them in a FAISS index for quick semantic search
5. Retrieves most relevant chunks based on a user query
6. Uses a generative QA model (e.g., FLAN‑T5) to produce natural responses

This setup allows a base transformer model to be **augmented with real context** for factual question answering.

---

## 🔧 Technologies Used

| Component                    | Description |
|-----------------------------|-------------|
| 📦 Wikipedia API            | Source for topic data |
| 🤗 Sentence Transformers    | Embeddings (`all‑mpnet‑base‑v2`) |
| 🧠 FAISS                    | Vector similarity search |
| 🛠 Hugging Face Transformers| Generative QA (`flan‑t5`) |
| 🧪 Python & Colab           | Notebook execution |
| 🌐 (Optional) Streamlit     | UI for interactive querying |

---

## 📌 How to Run

### 🧠 Run in Google Colab (recommended)
This notebook is fully compatible with Colab — click the badge above to run it instantly without setup.

### 🖥 Local Setup
If you want to run locally:

1. Clone the repo:
   ```bash
   git clone https://github.com/ritwik4m/rag-groq-streamlit.git
   cd rag-groq-streamlit

2. pip install -r requirements.txt
3. jupyter notebook Basic_RAG_pipeline.ipynb
