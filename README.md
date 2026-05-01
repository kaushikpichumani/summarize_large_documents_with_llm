# 📄 LLM-Based Document Summarization with LangChain & LangGraph

This project explores how to summarize **large documents and multiple files using LLMs (Large Language Models)**.

We demonstrate efficient techniques for handling long texts, chunking strategies, and optimizing prompts to generate concise and meaningful summaries. This approach is ideal for researchers, content analysts, and anyone looking to extract key insights from vast amounts of text quickly.

---

## 🚀 Overview

Large Language Models have token limits, making long-document summarization challenging.

This project solves that using a structured pipeline:
- Split large documents into chunks  
- Generate summaries for each chunk  
- Collapse intermediate summaries when needed  
- Produce a final concise summary  

---

## 🧩 Workflow

![Workflow Diagram](./output.png)


---

## ⚙️ Tech Stack

- 🦜 LangChain  
- 🔗 LangGraph  
- 🤖 LLMs (OpenAI or compatible models)  
- 🐍 Python  

---

## 🧠 Key Concepts

### 1. Chunking Strategy
Break large documents into smaller parts to fit within token limits.

```python
from langchain.text_splitter import RecursiveCharacterTextSplitter

splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=100)
chunks = splitter.split_text(document)

git clone <your-repo-url>
cd <your-repo>
pip install -r requirements.txt
export OPENAI_API_KEY=your_api_key

python main.py