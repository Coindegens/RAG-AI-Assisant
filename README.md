# GENERATIVE AI APP - LANGCHAIN AND RAG: AI RESEARCH QUERY ASSISTANT WITH WEB INTERFACE GRADIO

## Overview
An AI-powered RAG (Retrieval-Augmented Generation) assistant built with LangChain and Gradio web interface. This application optimizes research endeavors by processing documents, generating embeddings, and providing an interactive QA interface.

## Project Structure
```
langchain-rag-ai-assistant/
├── src/
│   └── tasks/
│       ├── document_loader.py
│       ├── text_splitter.py
│       ├── embedding.py
│       ├── vector_db.py
│       ├── retriever.py
│       ├── qa_bot.py
│       └── app.py
├── screenshots/
│   ├── code_splitter.png
│   ├── embedding.png
│   ├── QA_Bot_Interface.png
│   └── ...more screenshots
├── .venv-new/
├── requirements.txt
└── README.md
```

## Installation
To set up the project, follow these steps:

1. Clone the repository:
```bash
git clone <repository-url>
cd langchain-rag-ai-assistant
```

2. Create and activate virtual environment:
```bash
python -m venv .venv-new
.\.venv-new\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Task Implementations

### 1. Document Loader
- **File:** `src/tasks/document_loader.py`
- **Functionality:** Loads and processes PDF documents using LangChain
- **Output:** First 1000 characters of loaded content
- **Screenshot:** `screenshots/Task 1_pdf loader output.png`

### 2. Text Splitter
- **File:** `src/tasks/text_splitter.py`
- **Functionality:** Implements text splitting for enhanced model responsiveness
- **Feature:** Processes LATEX code and structured text
- **Screenshot:** `screenshots/code_splitter.png`

### 3. Embedding
- **File:** `src/tasks/embedding.py`
- **Functionality:** Generates embeddings using watsonx.ai API
- **Output:** Vector representations of text
- **Screenshot:** `screenshots/embedding.png`

### 4. Vector Database
- **File:** `src/tasks/vector_db.py`
- **Functionality:** Manages document embeddings and similarity searches
- **Screenshot:** `screenshots/vector_db.png`

### 5. Retriever
- **File:** `src/tasks/retriever.py`
- **Functionality:** Fetches relevant document segments based on queries
- **Screenshot:** `screenshots/retriever_output_1.png`

### 6. QA Bot
- **File:** `src/tasks/qa_bot.py`
- **Functionality:** Interactive QA interface with Gradio
- **Features:** Document upload, query processing
- **Screenshot:** `screenshots/QA_Bot_Interface.png`

## Requirements
- Python 3.13+
- LangChain
- PyPDF2
- Gradio
- Sentence Transformers
- Additional dependencies in requirements.txt

## Contributing
Contributions are welcome! Please submit a pull request or open an issue for any enhancements or bug fixes.

## License
This project is licensed under the MIT License.
