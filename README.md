# MediQA-RAG: Fine-Tuning & Retrieval-Augmented Generation for Medical Question Answering

## Project Summary
MediQA-RAG is a **Medical Question-Answering (QA) Bot** that leverages **Retrieval-Augmented Generation (RAG)** and fine-tunes the **T5-small** model on the **ChatDoctor dataset**. This project focuses on integrating fine-tuned language models with efficient document retrieval systems to deliver precise, context-aware responses in the medical domain. It also features an interactive **Gradio** interface for real-time medical Q&A.

### Key Features:
- **Fine-tuning T5-small** for medical domain-specific QA tasks.
- **RAG-based retrieval** using **FAISS** and **LangChain** to enhance contextual accuracy.
- **Interactive UI** with Gradio for seamless querying and real-time responses.
- **Performance tracking** via TensorBoard for model optimization.

---

## Project Report

### 1. Exploratory Data Analysis (EDA)
- Performed dataset analysis to identify key characteristics, such as **text length distributions** and **frequent medical terms**.
- Used **t-SNE** for embedding visualization, revealing natural clustering in the dataset.

### 2. Fine-Tuning the Model
- Attempted to fine-tune **Mistral-7B-OpenOrca** but shifted to **T5-small** due to GPU limitations.
- Applied **QLoRA (4-bit optimization)** techniques and tuned hyperparameters for efficiency.
- Used **Kaggle GPUs** over Colab due to session timeouts.

### 3. RAG-Based Retrieval System
- Deployed **FAISS** for similarity search and **LangChain** for RAG pipeline construction.
- Integrated **MiniLM embeddings** to improve search relevance.

### 4. Model Deployment & UI
- Built and deployed an intuitive **Gradio interface** for real-time interaction with the bot.
- Ensured efficient retrieval and response generation using **LangChain RetrievalQA**.

---
