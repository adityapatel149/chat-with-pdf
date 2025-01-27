# Multimodal RAG with LangChain: Chat-with-PDF

This project implements a **Multimodal Retrieval-Augmented Generation (RAG)** system using **LangChain**, **GROQ**, and **GPT-4o-mini** to enable natural language question answering from PDFs. By combining multimodal models and advanced language pipelines, the system can process text and images within PDFs, making it a versatile tool for extracting insights from complex documents.

## Features

- **Multimodal Question Answering**: Combines text and visual information from PDFs for precise answers.
- **LangChain Framework**: Orchestrates the document processing and conversational pipeline.
- **GROQ Integration**: Accelerates model inference, enhancing the system's speed.
- **GPT-4o-mini**: Provides high-quality, context-aware answers.

## Installation

To set up the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/chat-with-pdf.git
   cd chat-with-pdf
   ```
2. Ensure the following tools are installed on your system:
   - [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
   - Poppler utilities for PDF rendering

## Usage

1. Place your PDF files in the `content/` directory.

2. Run the notebook or script to start the system:
   ```bash
   jupyter notebook chat_with_pdf.ipynb
   ```

3. Interact with the chatbot by asking questions about the uploaded PDF documents.

## Key Components

### 1. PDF Processing
- **PyTesseract**: Extracts text from images embedded in PDFs.
- **pdf2image**: Converts PDF pages to images for multimodal analysis.
- **Unstructured.io**: Parses and structures text data from PDFs.

### 2. Multimodal RAG Pipeline
- **LangChain**: Chains together the document loader, vector store, and LLM.
- **GROQ**: Accelerates the embedding and question-answering processes.
- **GPT-4o-mini**: Generates accurate and contextually aware responses.

### 3. Vector Store
Uses a dense vector database (Chromadb) to store embeddings and retrieve relevant chunks for answering questions.

## Example Workflow

1. Upload a PDF document.
2. The system extracts text and images.
3. Relevant chunks are retrieved using the vector database.
4. The model generates an answer based on the retrieved information.

## Dependencies

Install the following Python packages:

```bash
pip install pytesseract poppler-utils pdf2image langchain langchain-community langchain-openai langchain-groq python-dotenv chromadb tiktoken pillow lxml
```

## Contributing

Contributions are welcome! If you'd like to improve this project, please:

1. Fork the repository.
2. Create a new branch.
3. Make your changes and submit a pull request.

## Acknowledgments

- **LangChain**: For the powerful framework.
- **GROQ**: For high-speed processing capabilities.
- **GPT-4o-mini**: For robust language understanding.

