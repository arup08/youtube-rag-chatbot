# YouTube RAG Chatbot 🎥🤖

This project implements a Retrieval-Augmented Generation (RAG) system that answers questions based on YouTube video transcripts.  
It uses LangChain, FAISS, and OpenAI models to build an intelligent chatbot over long-form video content.

## 🔧 Features

- 🧠 Converts YouTube video transcripts into semantically searchable chunks
- 🔍 Uses FAISS vector store for efficient similarity-based retrieval
- 💬 Answers user queries with accurate, context-aware responses from the video
- 🚀 Powered by OpenAI `text-embedding-3-small` and `gpt-4o-mini` LLM

## 📦 Tech Stack

- Python
- LangChain
- OpenAI API
- FAISS
- youtube-transcript-api

## 🚀 How It Works

1. **Transcript Ingestion**: Fetches transcript from YouTube using video ID.
2. **Text Chunking**: Splits the transcript into overlapping chunks.
3. **Embeddings**: Converts chunks into vectors using OpenAI embeddings.
4. **Vector Store**: Stores vectors in FAISS for fast similarity search.
5. **RAG Pipeline**: Retrieves relevant chunks and passes them to GPT-4o-mini for answering.

## 📝 Example Query

> **User:** Can you summarize the video?  
> **Bot:** [Generates a summary only from transcript content]
