# RAG-Chatbot
Build a conversational chatbot that can remember context and retrieve external information during conversations.  Dataset: Custom corpus (e.g., Wikipedia pages, internal documents, or any knowledge base)
# 🤖 Smart Multi-Source RAG Chatbot using Groq + LangChain

---

##  Project Overview
This project is a **Smart Multi-Source Retrieval-Augmented Generation (RAG) Chatbot** developed using *Streamlit, LangChain, FAISS, HuggingFace Embeddings, and Groq Llama 3.3 70B*.

The chatbot allows users to:
* 📤 **Upload PDF documents**
* 🌐 **Extract information from websites**
* 📖 **Fetch Wikipedia knowledge**
* 💬 **Ask intelligent questions**
* 🔍 **Retrieve relevant information**
* 🤖 **Generate AI-powered responses**

> **Note:** The system leverages semantic search and conversational AI to provide accurate, context-aware answers from multiple data sources simultaneously.

---

##  Objective
The main objective of this project is to build an intelligent chatbot capable of:
1. Reading and parsing PDF documents.
2. Understanding and scraping website content.
3. Retrieving Wikipedia summaries dynamically.
4. Performing high-speed semantic search.
5. Answering user queries with extreme accuracy.
6. Maintaining conversation history for multi-turn dialogues.

---

##  Technologies Used

| Component | Technology / Library | Role in Project |
| :--- | :--- | :--- |
| **UI Framework** | `Streamlit` | User Interface & Chat View |
| **Orchestration** | `LangChain` | RAG Pipeline & Workflow |
| **LLM Inference** | `Groq API` (Llama 3.3 70B) | Text Generation & Reasoning |
| **Vector Database** | `FAISS` | Similarity Search & Vector Storage |
| **Embeddings** | `HuggingFace Embeddings` | Converting Text to Vectors |
| **Data Loaders** | `PyPDFLoader` & `WebBaseLoader` | Extracting PDF & Web Content |
| **External API** | `Wikipedia REST API` | Fetching Wiki Knowledge Bases |
| **Text Splitter** | `RecursiveCharacterTextSplitter` | Chunking Document Data |
| **Memory** | `Session State` | Managing Conversational Context |

---

##  Project Workflow

### 1️⃣ Data Input
User uploads a PDF file, enters a website URL, or provides a Wikipedia topic through the Streamlit interface.

### 2️⃣ PDF Processing
The PDF text is extracted cleanly using `PyPDFLoader`.

### 3️⃣ Website Processing
Website content is scraped and loaded using `WebBaseLoader`.

### 4️⃣ Wikipedia Retrieval
Wikipedia summaries are fetched on-the-fly using the `Wikipedia REST API`.

### 5️⃣ Text Chunking
All collected text data is divided into smaller, manageable chunks using `RecursiveCharacterTextSplitter` for better retrieval accuracy.

### 6️⃣ Embedding Generation
Text chunks are converted into mathematical vector embeddings using HuggingFace embedding models.

### 7️⃣ Vector Storage
Embeddings are indexed and stored in a `FAISS` vector database for fast semantic similarity search.

### 8️⃣ User Query
The user asks a question related to the uploaded or retrieved knowledge base.

### 9️⃣ Context Retrieval
Relevant document chunks are retrieved from the FAISS vector database based on the query's semantic meaning.

### 🔟 Response Generation
The retrieved context and chat history are sent to **Llama 3.3 70B via Groq API** to generate a precise, human-like response.

---

##  Conversational Memory
The chatbot stores chat history using **Streamlit Session State**. This enables:
* 🔄 **Context-aware conversations** (the AI remembers what you said earlier).
* 🤝 **Better user interaction** through natural flow.
* 💬 **Multi-turn chatting** capabilities.

---

## ✨ Key Features
* 📄 **PDF Question Answering**
* 🌐 **Website Knowledge Extraction**
* 🌍 **Wikipedia Integration**
* 🚀 **Retrieval-Augmented Generation (RAG)**
* 🧠 **Conversational Memory**
* 🔍 **Semantic Search**
* ⚡ **Real-Time AI Responses**
* 🎨 **Streamlit Chat Interface**
* 📦 **Fast Retrieval using FAISS**
* 🔒 **URL Validation & Robust Error Handling**

---

##  Deployment
The application can be deployed seamlessly using:
* **Streamlit Cloud** (Native deployment)
* **Pyngrok** (For local tunneling and testing)

> `Pyngrok` generates a public URL, allowing you to share and access your locally running Streamlit chatbot online instantly.

---

##  Skills Gained
* Advanced **LangChain** workflow design
* End-to-End **RAG Architecture** implementation
* Vector operations with **FAISS Vector Database**
* Interactive **Streamlit Development**
* Designing **Conversational AI** systems
* **Prompt Engineering** for Llama models
* High-speed **LLM Integration** via Groq API
* Semantic Search & Text Embeddings
* Multi-Source Knowledge Retrieval

---

##  Conclusion
This project demonstrates how **RAG architecture** can be combined with Large Language Models (LLMs) to build an intelligent, multi-source chatbot capable of retrieving and generating accurate responses in real time.

By processing **PDFs, Websites, and Wikipedia data** under a unified pipeline and using **Groq Llama 3.3 70B**, this project provides a strong foundation for building advanced enterprise AI assistants and intelligent knowledge retrieval systems.

