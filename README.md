
---

# 🧠 Cold Email Generator using LangChain + Groq LLM

This project is an **AI-powered cold email generator** that utilizes **LangChain** with **Groq’s LLM APIs** to generate context-aware, tailored email drafts for job outreach or marketing purposes. By automating the process of cold email generation, this solution significantly reduces manual effort while improving personalization.

## 🚀 Features

* Uses **LangChain** with **Groq’s `mixtral-8x7b-32768` model**
* Supports **prompt-based generation** for cold emails or factual queries
* Lightweight and easy to adapt for personalized email campaigns
* Deployable in notebooks or production pipelines

## 🧰 Tech Stack

* **Python**
* **LangChain**
* **Groq API**

## 📦 Installation

To run this notebook, install the required dependencies:

```bash
pip install langchain-groq
```

We will also need:

```bash
pip install chromadb
```

## 🔑 Setup

We need a valid **Groq API key** to use the LLM:

```python
from langchain_groq import ChatGroq

llm = ChatGroq(
    model="mixtral-8x7b-32768",
    temperature=0,
    groq_api_key="your_groq_api_key"
)
```

## 📝 Usage Example

```python
response = llm.invoke("Write a cold email to apply for a data science internship at Google.")
print(response.content)
```

This will return a well-structured, relevant email response that you can refine and use.

## 📁 Structure

* `cold_email_generator.ipynb`: The main notebook containing the implementation and example prompt.


