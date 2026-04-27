# 🧠 RAG-based Legal Assistant – Live Build Project

This repository contains a live-built implementation of a context-aware legal assistant chatbot powered by advanced Retrieval-Augmented Generation (RAG) techniques. Instead of a polished tutorial, this project reflects a real-world development workflow using AI-assisted tools, iterative problem-solving, and practical system design.

---

## 🚀 Overview

The application processes legal documents and enables intelligent question-answering using a hybrid retrieval system that combines keyword-based and semantic search. It demonstrates how modern AI systems can be built to deliver accurate, context-grounded responses while adapting dynamically to query complexity.

---

## 🧠 Key Highlights

- Hybrid retrieval (BM25 + semantic vector search)  
- Multi-query and multi-hop reasoning  
- Reciprocal Rank Fusion (RRF) for improved ranking  
- AI-assisted development workflow  
- Real-time iteration and debugging  
- Conversation-aware chatbot with memory  
- Production-oriented architecture and evaluation  

---

## 📂 Project Structure

```
RAG-based-Legal-Assistant/
├── data/                           # Legal documents for indexing
├── modules/                        # Core RAG pipeline logic
├── prompts/                        # LLM prompt templates
├── outputs/                        # Generated outputs
├── RAGAS-dataset/                  # Evaluation datasets
├── app.py                          # Entry point
├── requirements.txt
└── README.md
```

---

## 🎥 How to Use This Repo

This is not a step-by-step tutorial. To get the most out of it:

1. Clone the repository  
2. Explore modules step-by-step  
3. Run the application and test queries  
4. Modify retrieval strategies and observe behavior  
5. Focus on understanding system design, not just execution  

---

## ⚙️ Getting Started

```bash
git clone https://github.com/deepanshuopxd/RAG-Legal-Assistant.git
cd RAG-Legal-Assistant
```

Install dependencies:

```bash
pip install -r requirements.txt
# or
uv sync
```

Run the application:

```bash
uv run app.py
# or
python app.py
```

---

## 🔧 Configuration

Create a `.env` file and add your API keys:

```env
COHERE_API_KEY=your_cohere_api_key_here
OPENAI_API_KEY=your_openai_api_key_here
```

⚠️ Do not commit your `.env` file.

---

## 🧩 How It Works

### 1. Document Processing
- Loads and splits legal PDFs  
- Generates embeddings using HuggingFace models  
- Stores them in a vector database  

### 2. Retrieval System
- Combines BM25 (keyword search) + semantic retrieval  
- Expands queries using multi-query generation  
- Handles complex reasoning via multi-hop retrieval  
- Merges results using Reciprocal Rank Fusion (RRF)  

### 3. Response Generation
- Uses LLM (Cohere/OpenAI) for answer generation  
- Grounds responses in retrieved context  
- Maintains conversation history for continuity  

---

## 🎯 Learning Goals

- Understand Retrieval-Augmented Generation (RAG) systems  
- Learn hybrid search and ranking techniques  
- Explore AI-assisted development workflows  
- Gain experience with real-world debugging and iteration  
- Build intuition for production-ready AI applications  

---