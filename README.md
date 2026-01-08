# medical-chatbot-rag-llm
A symptom-based medical assistant built using RAG architecture and fine-tuned Llama-2-7B.

# 🏥 Medical Chatbot using RAG and Fine-Tuned LLMs

## 📌 Project Overview
[cite_start]Developed as part of the **National Student Data Corps (NSDC)** project series[cite: 35, 36]. This project implements a multi-stage chatbot that evolved from a rule-based system into a sophisticated **Retrieval-Augmented Generation (RAG)** architecture using **Llama-2**.

## 🛠️ Technical Implementation (X-Y-Z)
* [cite_start]**Accomplishment (X):** Developed a medical chatbot capable of interpreting natural language symptoms and suggesting possible conditions[cite: 43].
* **Quantifiable Result (Y):** Optimized LLM performance via **4-bit Quantization (QLoRA)**, allowing a **7B parameter model** to run efficiently on a single **T4 GPU**.
* **Method (Z):** Utilized `Python`, `PyTorch`, and `Hugging Face`; implemented `SentenceTransformers` for vector embeddings and semantic search.

## 🧪 Key Features
* **RAG Architecture:** Prevents hallucinations by retrieving context from a curated medical dataset before generating responses.
* **PEFT/LoRA Fine-tuning:** Updated only a small subset of model weights to adapt the LLM to specific medical symptom-disease pairs.
* **Semantic Search:** Used `cosine similarity` to match user inputs with vector-embedded medical records.

## 📜 Certification
* [cite_start]**Project Completion Certificate:** Awarded by the *Northeast Big Data Innovation Hub*[cite: 35, 38].
