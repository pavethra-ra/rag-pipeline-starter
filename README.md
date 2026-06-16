# RAG Pipeline Starter 🤖

End-to-end Retrieval-Augmented Generation 
pipeline using Python and LangChain.

## 🎯 What This Does

- 📄 Loads documents (PDF, TXT, Word)
- 🔢 Generates embeddings using OpenAI
- 🗄️ Stores in FAISS vector database
- 🔍 Retrieves relevant context for queries
- 🤖 Generates accurate AI responses

## 🛠️ Tech Stack

- Python 3.11+
- LangChain
- FAISS (Vector Database)
- OpenAI API
- PyPDF2

## 🚀 Quick Start

# 1. Clone the repository
git clone https://github.com/pavethra-ra/rag-pipeline-starter.git
cd rag-pipeline-starter

# 2. Install dependencies
pip install -r requirements.txt

# 3. Setup environment variables
cp .env.example .env
# Add your OpenAI API key to .env

# 4. Run the demo
python examples/demo.py

## 📁 Project Structure

rag-pipeline-starter/
├── src/
│   ├── rag_pipeline.py      # Main RAG class
│   ├── document_loader.py   # Document loaders
│   └── embeddings.py        # Embedding utilities
├── examples/
│   └── demo.py              # Usage example
├── requirements.txt
└── README.md

## 💡 Example Usage

```python
from src.rag_pipeline import RAGPipeline

# Initialize RAG pipeline
rag = RAGPipeline()

# Load documents
rag.load_documents("data/sample_docs/")

# Query
response = rag.query("What is the main topic?")
print(response)
```

## 🔧 Configuration

Edit .env file:
- OPENAI_API_KEY=your_key_here
- CHUNK_SIZE=500
- CHUNK_OVERLAP=50

## 📚 Topics Covered

- ✅ Document ingestion and chunking
- ✅ Embedding generation
- ✅ Vector database operations
- ✅ Similarity search
- ✅ LLM-powered response generation

## 🤝 Contributing

Contributions welcome! Open an issue 
or submit a PR.

## 📝 License

MIT License

## 👩‍💻 Author

**Pavithra R**  
Senior Python AI Engineer  
🔗 [LinkedIn](https://www.linkedin.com/in/pavithra-r-55536182)  
📧 pavithra0849@gmail.com

⭐ Star this repo if helpful!
