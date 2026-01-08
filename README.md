# 🏥 Medical Chatbot using RAG and Fine-Tuned LLMs

## 📌 Project Overview
[cite_start]Developed as part of the **National Student Data Corps (NSDC)** project series[cite: 37, 43]. This project implements a multi-stage chatbot that evolved from a rule-based system into a sophisticated **Retrieval-Augmented Generation (RAG)** architecture using **Llama-2**.

## 🛠️ Technical Implementation (X-Y-Z)
* **Accomplishment (X):** Developed a medical chatbot capable of interpreting natural language symptoms and suggesting possible conditions.
* **Quantifiable Result (Y):** Optimized LLM performance via **4-bit Quantization (QLoRA)**, allowing a **7B parameter model** to run efficiently on a single **T4 GPU**.
* **Method (Z):** Utilized `Python`, `PyTorch`, and `Hugging Face`; implemented `SentenceTransformers` for vector embeddings and semantic search.

## 🧪 Key Features
* **RAG Architecture:** Prevents hallucinations by retrieving context from a curated medical dataset before generating responses.
* **PEFT/LoRA Fine-tuning:** Updated only a small subset of model weights to adapt the LLM to specific medical symptom-disease pairs.
* **Semantic Search:** Used `cosine similarity` to match user inputs with vector-embedded medical records.

## 🚀 How to Run Locally
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/PemaDT/medical-chatbot-rag-llm.git](https://github.com/PemaDT/medical-chatbot-rag-llm.git)

2. Install dependencies:
   
   pip install -r requirements.txt
   
4. Run the Notebook: Open medical-chatbot-updated.ipynb in Kaggle or a local Jupyter environment with GPU support.


## 🏆 Certification
View the official **Certificate of Completion** from the *Northeast Big Data Innovation Hub* and *National Student Data Corps* here: 
[📄 Click to view Certificate](./Certificate%20of%20DSP%20Completion%20-%20MedChat.pdf)

## 📊 Technical Benchmarks & Findings

While this project serves as a technical proof-of-concept, the following engineering milestones were achieved:

* **Model Compression (Quantization):** Successfully reduced the memory footprint of the Llama-2-7B model from ~28GB to **under 5GB** using **4-bit NormalFloat (NF4)** quantization.
* **Hardware Efficiency:** Optimized the pipeline to run a 7-billion parameter model on a **single T4 GPU** (16GB VRAM), a 75% reduction in typical hardware requirements.
* **Factually Grounded Responses:** Implementing **RAG** significantly reduced model "hallucinations" by restricting the LLM's knowledge base to provided medical records during the inference phase.
* **Parameter Efficiency:** Utilizing **QLoRA** allowed for fine-tuning by updating less than 1% of the model's total parameters, drastically reducing training time and compute costs.
