# CI_2025
An AI-powered research assistant that automates paper retrieval from arXiv, creates local vector embeddings for semantic search, and generates source-verified answers using Llama 3. It features a professional Streamlit dashboard that provides executive summaries and direct PDF links for evidence-based scholarly analysis.



AI Research Analyzer
An advanced RAG (Retrieval-Augmented Generation) application designed for scholarly analysis. This tool connects to the arXiv API, downloads relevant research papers, indexes them into a local vector database, and uses Llama 3 (via Ollama) to provide precise, source-backed answers to complex research questions.

Key Features
Real-time arXiv Integration: Automatically fetches and parses the latest PDF research papers.

Executive Summarization: Generates a high-level overview of multiple papers using LLMs.

Local Vector Storage: Uses ChromaDB and HuggingFace embeddings for efficient semantic search.

Source Verification: Provides direct clickable links to the specific papers and page numbers used to generate answers.

Modern UI: A sleek, dark-themed Streamlit interface with glassmorphism effects.
Tech Stack
LLM Orchestration: LangChain

Model: Llama 3 (running locally via Ollama)

Embeddings: sentence-transformers/all-mpnet-base-v2

Vector Database: ChromaDB

Frontend: Streamlit

Data Source: arXiv API

Getting Started
Prerequisites
Install Ollama: Download from ollama.com.

Pull Llama3: Run ollama pull llama3 in your terminal.

Python 3.9+

Installation
Clone the repository:

Bash
pip install -r requirements.txt
Set up Environment: Create a .env file (if you plan to use OpenAI models, otherwise the current setup uses Ollama).

Running the App
Bash
streamlit run app.py
Usage
Enter a Topic: (e.g., "Quantum Error Correction")

Ask a Question: (e.g., "What are the latest surface code thresholds?")

Deep Research: The app will download papers, index them, and provide a verified answer with sources.
