# KnowledgeLens

KnowledgeLens is a Retrieval-Augmented Generation (RAG) system that transforms PDF documents into searchable knowledge repositories. The application combines semantic embeddings, vector similarity search, LangChain, and Groq LLMs to retrieve relevant context from documents and generate accurate, context-grounded responses.

## Overview

KnowledgeLens demonstrates the complete RAG workflow, from document ingestion to answer generation. Instead of relying solely on a language model's pre-trained knowledge, the system retrieves relevant information from source documents and augments the model's context before generating a response. This approach improves factual accuracy and reduces hallucinations.

## Architecture

```text
PDF Documents
      │
      ▼
Document Loader
      │
      ▼
Text Chunking
      │
      ▼
Embedding Generation
      │
      ▼
Vector Database
      │
      ▼
Semantic Retrieval
      │
      ▼
Prompt Augmentation
      │
      ▼
Groq LLM
      │
      ▼
Generated Response
```

## Features

- PDF document processing
- Text chunking and preprocessing
- Embedding generation
- Vector-based semantic search
- Retrieval-Augmented Generation (RAG)
- Context-aware question answering
- LangChain integration
- Groq LLM integration

## Technology Stack

- Python
- LangChain
- Groq
- Vector Database
- Jupyter Notebook

## Project Structure

```text
KnowledgeLens/
│
├── data/
├── notebook/
│   ├── document.ipynb
│   └── pdf_loader.ipynb
├── src/
│   └── __init__.py
├── main.py
├── pyproject.toml
├── requirements.txt
├── uv.lock
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/404prateek/KnowledgeLens.git
cd KnowledgeLens
```

Create and activate a virtual environment:

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

Linux/macOS:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Configuration

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key
```

## Running the Application

```bash
python main.py
```

## Key Concepts

- Retrieval-Augmented Generation (RAG)
- Semantic Search
- Vector Embeddings
- Document Processing
- Prompt Augmentation
- Large Language Models
- Context Grounding

## Future Improvements

- Web-based user interface
- Multi-document retrieval
- Conversational memory
- Hybrid retrieval strategies
- Source citation support
- Cloud deployment

## License

This project is available under the MIT License.
