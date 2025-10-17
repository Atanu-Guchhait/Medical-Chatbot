🧠 Medicinal Chatbot — RAG-Powered Healthcare Assistant

An intelligent Medicinal Chatbot built using Retrieval-Augmented Generation (RAG) pipeline.
This system processes PDFs of medicinal or healthcare data and provides context-aware, conversational answers using DeepSeek-R1-Distill-LLaMA-70B and a hybrid Ensemble Retriever system.

🚀 Features

✅ Reads and processes medical PDFs using PyPDFLoader
✅ Efficiently splits long documents with RecursiveCharacterTextSplitter
✅ Creates semantic embeddings using Sentence Transformers
✅ Stores & retrieves data using ChromaDB
✅ Uses DeepSeek-R1-Distill-LLaMA-70B for reasoning and response generation
✅ Employs Ensemble Retriever for hybrid search (dense + keyword)
✅ Maintains context through ConversationalBufferMemory
✅ Interactive user loop for real-time chat

🏗️ Architecture Overview
            ┌────────────────────────────┐
            │     Medicinal PDFs         │
            └────────────┬───────────────┘
                         │
               PyPDFLoader (DirectoryLoader)
                         │
          RecursiveCharacterTextSplitter
                         │
         Sentence-Transformer Embeddings
                         │
                    ChromaDB Vector Store
                         │
                Ensemble Retriever (Dense + Sparse)
                         │
            ChatPromptTemplate + DeepSeek-R1-70B
                         │
           ConversationalBufferMemory (History)
                         │
               Interactive Chat Interface

🧩 Tech Stack
Component	Technology
Document Loading	DirectoryLoader, PyPDFLoader
Chunking	RecursiveCharacterTextSplitter
Embeddings	sentence-transformers/all-MiniLM-L6-v2
Vector Store	ChromaDB
Retriever	EnsembleRetriever (combining BM25 + Vector Search)
LLM	deepseek-r1-distill-llama-70b
Prompt Management	ChatPromptTemplate
Memory	ConversationalBufferMemory
Interface	Interactive Python Loop / Streamlit Chat UI
