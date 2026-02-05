# MediBot🩺 – AI Powered RAG Medical Chatbot

## Project Overview

MediBot is an AI-powered conversational chatbot built using Retrieval Augmented Generation (RAG) architecture. The system allows users to ask questions and receive accurate responses based strictly on a predefined knowledge base instead of generating random answers.

The chatbot retrieves relevant information from a vector database using semantic search and combines it with a Large Language Model (LLM) to generate context-aware responses.

This project demonstrates the integration of modern AI technologies, including vector databases, embeddings, and LLM orchestration using LangChain.


## Problem Statement
Traditional chatbots often generate hallucinated responses because they rely only on pretrained knowledge. This project solves that problem by:
* Retrieving real information from a structured knowledge base
* Restricting answers strictly to retrieved context
* Improving accuracy and reliability


## Key Features
* Retrieval Augmented Generation (RAG) pipeline
* Semantic search using FAISS vector database
* HuggingFace embeddings for contextual understanding
* Groq LLM integration (Llama model)
* Chat-based interactive UI using Streamlit
* Context-based answering (no hallucinated responses)
* Session-based chat history


## Architecture

System workflow:
1. User enters a question in Streamlit interface
2. Question is converted into embeddings
3. FAISS vector database retrieves relevant documents
4. Retrieved context is passed to LLM through prompt template
5. LLM generates final response using only provided context
6. Answer displayed in chatbot UI


## Tech Stack

Programming Language:

* Python

Frameworks & Libraries:

* Streamlit
* LangChain
* FAISS
* HuggingFace Embeddings
* Groq API (Llama model)
* Sentence Transformers
* Scikit-learn


## Project Structure

```
project/
│
├── medibot.py          # Main chatbot application
├── vectorstore/        # FAISS vector database
├── requirements.txt
├── .env                # API keys
└── README.md

```

## How It Works (Technical Explanation)

* HuggingFace sentence-transformer converts text into embeddings.
* FAISS stores and retrieves similar documents using vector similarity.
* LangChain builds retrieval pipeline.
* Groq LLM generates answer based on retrieved context.
* Custom prompt ensures no information is generated outside context.

---

## Example Use Cases

* Medical knowledge assistant
* Domain-specific chatbot
* Knowledge-base QA system
* Research assistant chatbot

---

## Future Improvements

* Add memory persistence
* Multi-document upload support
* Cloud deployment (AWS / GCP)
* Authentication system
* Source document highlighting

---

## License

MIT License

---




