# 🎥 YTInsight-- Intelligent YouTube Q&A with RAG

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Build](https://img.shields.io/badge/Build-Passing-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![LLM](https://img.shields.io/badge/LLM-OpenAI%20%7C%20GoogleAI-purple)
![Framework](https://img.shields.io/badge/Framework-LangChain-orange)

------------------------------------------------------------------------

## 📌 Overview

YTBot is an AI-powered YouTube assistant that converts video transcripts
into an interactive question-answering system using
**Retrieval-Augmented Generation (RAG)**.

It enables users to: - Extract transcripts from YouTube videos\
- Perform semantic search over video content\
- Generate context-aware responses using LLMs\
- Interactively query long-form video content

------------------------------------------------------------------------

## 🧠 System Architecture

The system follows a modern Retrieval-Augmented Generation pipeline:

![Architecture Diagram](<img width="1536" height="1024" alt="architecture png" src="https://github.com/user-attachments/assets/bae8261f-8b71-43ac-b955-57848ef0052d" />)

### 🔄 Pipeline Flow

1.  **YouTube URL Input**\
2.  **Transcript Extraction** (YouTube Transcript API)\
3.  **Text Chunking & Embedding Generation**\
4.  **Vector Database Storage** (FAISS / ChromaDB)\
5.  **Semantic Retrieval**\
6.  **LLM Response Generation** (OpenAI / Google AI)\
7.  **Contextual Answer Output**

This ensures responses are grounded strictly in video context,
minimizing hallucinations.

------------------------------------------------------------------------

## 🚀 Features

-   🎥 YouTube transcript extraction\
-   🔎 Vector-based semantic retrieval\
-   🧠 Context-aware AI responses\
-   📚 Long-form content understanding\
-   ⚡ Modular RAG architecture

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   **Language:** Python 3.9+\
-   **Framework:** LangChain\
-   **LLM Providers:** OpenAI / Google Generative AI\
-   **Vector Store:** FAISS / ChromaDB\
-   **API:** YouTube Transcript API

------------------------------------------------------------------------

## ⚙️ Installation

``` bash
git clone https://github.com/your-username/ytbot.git
cd ytbot
```

Create a virtual environment:

``` bash
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows
```

Install dependencies:

``` bash
pip install langchain openai faiss-cpu youtube-transcript-api chromadb python-dotenv
```

------------------------------------------------------------------------

## 🔐 Environment Variables

Create a `.env` file:

For OpenAI:

    OPENAI_API_KEY=your_api_key

For Google:

    GOOGLE_API_KEY=your_api_key

------------------------------------------------------------------------

## ▶️ Usage

1.  Open `ytbot.ipynb`
2.  Run all cells
3.  Provide a YouTube video URL
4.  Ask questions interactively

Example:

``` python
"What are the key takeaways from this lecture?"
```

------------------------------------------------------------------------

## 📈 Future Enhancements

-   Web deployment (FastAPI / Streamlit)\
-   Multi-video knowledge base\
-   Conversational memory\
-   CI/CD integration\
-   Cloud deployment

------------------------------------------------------------------------

## 📜 License

This project is licensed under the MIT License.
