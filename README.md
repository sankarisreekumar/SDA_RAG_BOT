SDA RAG Chatbot — Query Answering with ChromaDB + Sentence Transformers + Qwen LLM

This project implements a Retrieval-Augmented Generation (RAG) chatbot for the School of Data Analytics (SDA).
It allows users to ask questions related to syllabus, fees, faculty, electives, and infrastructure—and provides answers strictly based on the uploaded text files.

The system uses:

ChromaDB → As the vector database

SentenceTransformer (all-MiniLM-L6-v2) → For embedding text and queries

Qwen2.5-1.5B-Instruct → As the local LLM for generating context-aware answers

Python (Colab) → For loading text, embedding, storing vectors, and generating responses

🚀 Features
✅ 1. Automatic Text Loading

Loads and reads multiple SDA-related text files such as:

DSA program details

Faculty information

Fee & infrastructure

Syllabus

Electives

✅ 2. Chunk Embedding

Each document is embedded using all-MiniLM-L6-v2 and stored in ChromaDB.

✅ 3. Semantic Retrieval

For any query, the system retrieves the most relevant text chunks using vector similarity search.

✅ 4. LLM-Based Answer Generation

Uses Qwen2.5-1.5B-Instruct to generate accurate answers using the retrieved context.

The responses strictly use the relevant context.
If no answer is found → returns “No data found.”
