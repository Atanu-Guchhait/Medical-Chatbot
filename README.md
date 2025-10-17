
 🧠 Medicinal Chatbot — RAG-Powered Healthcare Assistant



This project is an intelligent medicinal chatbot built using a Retrieval-Augmented Generation (RAG) pipeline.
It can read medicinal or healthcare PDFs, understand them, and answer user queries in a conversational manner using the DeepSeek-R1-Distill-Llama-70B model.

>>>>>>>>>>>>>>>>>>>Features

✅Loads and processes medical PDFs using PyPDFLoader

✅Splits long documents using RecursiveCharacterTextSplitter

✅Generates semantic embeddings using SentenceTransformer

✅Stores and retrieves data using ChromaDB

✅Uses DeepSeek-R1-Distill-Llama-70B for response generation

✅Uses Ensemble Retriever for hybrid (dense + keyword) search

✅Maintains conversation history with ConversationalBufferMemory

✅Provides an interactive user chat loop

>>>>>>>>>>>>>>>>>>>>>>>>Architecture Workflow

Load medicinal PDFs using DirectoryLoader and PyPDFLoader

✅Split the text into smaller chunks using RecursiveCharacterTextSplitter

✅Generate embeddings using SentenceTransformer

✅Store embeddings in ChromaDB (vector database)

✅Retrieve relevant information using EnsembleRetriever

✅Use ChatPromptTemplate to build dynamic conversation prompts

✅Maintain conversation history using ConversationalBufferMemory

✅Use DeepSeek-R1-Distill-Llama-70B for intelligent responses

✅Output responses through an interactive chat loop

>>>>>>>>>>>>>>>>>Components and Tools

✅DirectoryLoader

✅PyPDFLoader

✅RecursiveCharacterTextSplitter

✅SentenceTransformer Embedding

✅ChromaDB

✅EnsembleRetriever

✅DeepSeek-R1-Distill-Llama-70B

✅ChatPromptTemplate

✅ConversationalBufferMemory
