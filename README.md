# 📄 PDF-RAG FastAPI

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-async--powered-green?logo=fastapi)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Open Source Love](https://img.shields.io/badge/Open%20Source-%E2%9D%A4-red)

**PDF-RAG FastAPI** is a lightweight and production-ready Retrieval-Augmented Generation (RAG) application that allows users to upload PDFs and interactively query them via a powerful language model—all accessible through a FastAPI endpoint.

---

## 🚀 Features

- 🔍 **PDF-based Document Understanding** using LLMs  
- 🧠 **RAG Architecture** with embedding-based retrieval  
- ⚡ **FastAPI Backend** for lightweight serving  
- 🧩 **Local Embedding Model** for cost-effective deployment (no OpenAI key needed)  
- 📦 Simple to extend with Docker or Streamlit UI (future updates)

---

## 📂 Project Structure

```bash
.
├── app/
│   ├── main.py              # FastAPI app
│   ├── rag_engine.py        # Embedding + Query engine
│   ├── utils.py             # Helper functions (PDF parsing, etc.)
│
├── sample_pdfs/             # Folder to hold uploaded PDFs
├── requirements.txt
├── README.md
