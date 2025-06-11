# 🧠 Local RAG Chatbot - Pizza Reviews 🍕

This is a lightweight Retrieval-Augmented Generation (RAG) demo using [LangChain](https://github.com/langchain-ai/langchain), [Ollama](https://github.com/ollama/ollama), [Chroma](https://github.com/chroma-core/chroma), and [LLaMA 3](https://ollama.com/library/llama3). It answers questions based on real-world restaurant review data.

---

## 🔍 Features

- 🔗 RAG pipeline using LangChain
- 🧠 Local inference via Ollama + LLaMA 3
- 💾 Embedding-based retrieval with ChromaDB
- 📄 Input data from realistic restaurant reviews (CSV)
- 🖥️ Simple command-line interface

---

## 📦 Prerequisites

- Python 3.10+
- [Ollama](https://ollama.com) installed and running
- Pull required models:
  \`\`\`
  ollama pull llama3
  ollama pull mxbai-embed-large
  \`\`\`

---

## ⚙️ Setup

\`\`\`
git clone https://github.com/BhagyeshPatil2004/local-rag-pizza-chatbot.git
cd local-rag-pizza-chatbot
python -m venv .venv
source .venv/bin/activate   # or use .venv\Scripts\activate on Windows
pip install -r requirements.txt
\`\`\`

---

## 🚀 Run the App

\`\`\`
python RAG/main.py
\`\`\`

You’ll be prompted to ask questions like:

\`\`\`
Ask your question (q to quit): tell me pizza under \$25
\`\`\`

---

## 📁 Project Structure

\`\`\`
├── RAG/

│   ├── main.py           # CLI-based chatbot logic

│   ├── vector.py         # Embedding + Chroma setup

├── realistic_restaurant_reviews.csv  # Input review dataset

├── requirements.txt      # Python dependencies

└── README.md             # This file
\`\`\`

---

## 🧪 Sample Questions

- "Tell me pizza under \$25"
- "How are the vegan options?"
- "What do reviews say about customer service?"

---

## 📌 Notes

- No OpenAI API key is needed.
- All models and data processing are **100% local**.
- You can swap the dataset or tweak the prompt template for other domains.

---

## 👨‍💻 Author

[Bhagyesh Patil](https://github.com/BhagyeshPatil2004)
