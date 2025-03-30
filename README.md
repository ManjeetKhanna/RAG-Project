# RAG-Project

## Overview
This project builds an AI-powered Retrieval-Augmented Generation (RAG) system that extracts relevant information from scientific research papers and generates insightful responses. The integration of Pinecone, OpenAI's GPT-4o-mini, and Streamlit enhances access to scientific knowledge. The system uses advanced semantic search to ensure that the generated content is both accurate and contextually appropriate.

## Objective
- Enable AI-driven semantic search and response generation for research papers.
- Utilize Retrieval-Augmented Generation (RAG) to enhance factual accuracy and coherence.
- Improve response faithfulness using context-aware retrieval techniques.

## Technology Framework
- OpenAI GPT-4o-mini – AI-powered response generation
- Pinecone – Scalable vector search for retrieval
- SentenceTransformers (all-mpnet-base-v2) – Embedding model for text chunking
- Streamlit – Interactive UI for user interaction
- Ragas Evaluation – Automated performance assessment

## Working Mechanism
- Text Ingestion & Processing: Extracts content from research papers (PDFs) and splits it into meaningful chunks.
- Embedding Generation: Converts text into dense vectors using SentenceTransformers.
- Vector Storage & Retrieval: Stores embeddings in Pinecone and retrieves relevant text upon query.
- Response Generation: Uses GPT-4o-mini to generate AI responses based on retrieved context.
- Evaluation Metrics: Measures performance with context recall, faithfulness, and factual correctness.

## Setup and Implementation
### 1. Install dependencies
```bash
   pip install -r requirements.txt```

### 2. Set Up Environment Variables
   Create a .env file and add the following:
   ```bash
    OPENAI_API_KEY=your_openai_key
    PINECONE_API_KEY=your_pinecone_key
    PINECONE_INDEX_HOST=your_pinecone_host```

### 3. Run the Application
```bash
   streamlit run streamlit.py```
