# 🤖 Mini RAG Q&A Chatbot

Mini RAG Q&A is a simple AI project that lets you add your own document and ask questions about it.

Instead of giving the AI a question directly, the project first looks for the most relevant parts of the document and then uses them to generate an answer. This makes it useful for things like studying notes, articles, or other text-based documents.

## What does it do?

You can:

- Paste a document into the app
- Store the document in ChromaDB
- Ask questions about the document
- Find the most relevant parts of the document
- Get an answer from a local AI model
- View the information that was used to generate the answer

## How it works

The project follows a simple RAG workflow:

**Document → Split into chunks → Create embeddings → Store in ChromaDB → Ask a question → Find relevant chunks → Generate answer with Ollama**

The document is divided into smaller chunks and converted into embeddings using Sentence Transformers. These embeddings are stored in ChromaDB, which helps find the parts of the document that are most relevant to a question.

The relevant information is then given to **Llama 3.2 through Ollama**, which generates the final answer.

## Technologies Used

- Python
- Streamlit
- Sentence Transformers
- ChromaDB
- Ollama
- Llama 3.2

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Hasininimmakayala/mini-rag-qa-chatbot.git
cd mini-rag-qa-chatbot
