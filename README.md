# 🔊 Voice Conversational Agentic AI

This project is a Python-based RESTful API that enables **two-way voice conversations** with a Large Language Model (LLM), enhanced using **Retrieval Augmented Generation (RAG)**. Users can speak to the system, receive intelligent voice responses, and upload custom documents (PDF, TXT, CSV, JSON) that the model can use to give better answers.

---

## 🚀 Features

- 🎤 Real-time voice input and transcription via STT APIs (OpenAI Whisper, Google Cloud, Azure)
- 🧠 LLM with memory using OpenAI GPT or similar APIs
- 📄 Document upload and vector indexing with FAISS, Pinecone, or Weaviate
- 🔍 Context-aware Retrieval Augmented Generation (RAG)
- 🗣️ Text-to-speech conversion with OpenAI TTS, Google TTS, or Amazon Polly
- 🧩 Clean RESTful API design for modular usage

---

## 📦 API Endpoints

| Endpoint            | Method | Description |
|---------------------|--------|-------------|
| `/transcribe`       | POST   | Accepts voice input, returns text and STT time |
| `/chat`             | POST   | Sends conversation and new message to LLM, returns response |
| `/speak`            | POST   | Converts text to audio, returns TTS time |
| `/converse`         | POST   | End-to-end voice → LLM + RAG → voice |
| `/reset`            | POST   | Clears LLM conversation memory |
| `/upload_rag_docs`  | POST   | Uploads documents for RAG knowledge base |

---

## 🛠️ Tech Stack

- **FastAPI** – Backend framework
- **OpenAI / Whisper / Google Cloud** – Speech-to-Text (STT)
- **OpenAI GPT / Azure OpenAI** – LLM
- **FAISS / Pinecone / Weaviate** – Vector stores for RAG
- **OpenAI TTS / Amazon Polly / Google TTS** – Text-to-Speech
- **Docker** – Optional containerization
- **Uvicorn** – ASGI server

---

## 📂 Getting Started

1. **Clone the Repo**
   ```bash
   git clone https://github.com/YOUR-USERNAME/voice-agent-ai.git
   cd voice-agent-ai

