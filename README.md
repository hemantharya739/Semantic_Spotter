
# Semantic Spotter: Generative Search System for Policy Documents

## Overview
Semantic Spotter is a robust generative search system designed to deliver accurate and contextually relevant responses to queries based on policy documents. It leverages LangChain's Retrieve-and-Generate (RAG) architecture, integrating document chunking, semantic embeddings, vector storage, and reranking mechanisms.

## Features
- PDF ingestion and chunking using LangChain
- Semantic embeddings via OpenAIEmbeddings
- Vector storage with ChromaDB
- Intelligent retrieval using MMR strategy
- Re-ranking with HuggingFace CrossEncoder (BAAI/bge-reranker-base)
- RAG chain integration using LangChain chains and prompts

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/semantic-spotter.git
   cd semantic-spotter
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scriptsctivate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Add your policy documents to the `Policy+Documents` folder.

5. Run the main script or notebook to start querying.

## Usage
Use the `get_topk_relevant_documents(query, topk)` function to retrieve and rerank documents based on your query.

## License
This project is licensed under the MIT License.
