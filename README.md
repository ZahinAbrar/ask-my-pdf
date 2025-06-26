
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
```

---

## ⚙️ Installation

### 🔧 Setup (Local/Colab)

1. Clone the repo:
```bash
git clone https://github.com/your-username/pdf-rag-fastapi.git
cd pdf-rag-fastapi
```

2. Install requirements:
```bash
pip install -r requirements.txt
```

3. Run the FastAPI server:
```bash
uvicorn app.main:app --reload
```

---

## 📤 API Usage

### 🔗 Endpoint: `/query`

- **Method:** `POST`
- **Payload:**
```json
{
  "pdf_path": "sample_pdfs/Graphical_Lasso.pdf",
  "query": "What is the main idea of the document?"
}
```

- **Response:**
```json
{
  "answer": "The document discusses Graphical Lasso for sparse inverse covariance estimation..."
}
```

---

## 📚 Example Use Cases

- Research paper Q&A
- Legal document summarization
- Financial report interpretation
- Automating knowledge extraction from manuals

---

## 🤝 Contributing

We welcome contributions! Please open an issue or submit a PR with improvements, bug fixes, or ideas for enhancements.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## ✨ Acknowledgements

Built using:
- [FastAPI](https://fastapi.tiangolo.com/)
- [LlamaIndex](https://github.com/jerryjliu/llama_index)
- [HuggingFace Transformers](https://huggingface.co/)

---

## 🌍 Let's Build RAG Apps for Everyone

> If you find this helpful, feel free to ⭐ the repo and share it!
