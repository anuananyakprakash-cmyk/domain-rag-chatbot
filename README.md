# Domain-Specific RAG Chatbot

## Project Description
This project is a Domain-Specific Retrieval-Augmented Generation (RAG) chatbot that answers questions using information from uploaded PDF documents.

## Technologies Used
- Python
- Streamlit
- Ollama (Qwen2.5 1.5B)
- Sentence Transformers
- FAISS
- PyPDF
- LangChain Text Splitters

## Features
- Extracts text from PDF documents.
- Splits text into smaller chunks.
- Retrieves relevant information using FAISS.
- Generates answers using a local language model.
- Displays source document information.
- Avoids answering unsupported questions.

## How It Works
PDF Document → Text Extraction → Text Chunking → Embeddings → FAISS Search → Ollama → Answer

## How to Run
1. Install the dependencies using `pip install -r requirements.txt`.
2. Install Ollama separately and download the model using `ollama pull qwen2.5:1.5b`.
3. Start the application using `streamlit run app.py`.

## Project Files
- `app.py` – Main Streamlit application
- `document_loader.py` – PDF text extraction
- `vector_store.py` – Vector database and retrieval
- `rag_pipeline.py` – RAG processing
- `prompt.py` – Prompt instructions
- `requirements.txt` – Python dependencies
- `architecture.png` – Architecture diagram
- `testing_sheet.csv` – Testing results
- `documents/` – Sample PDF documents
