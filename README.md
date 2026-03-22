# AskMyPDF-Gemini-RAG-

## 📌 Description

This project is a **Retrieval-Augmented Generation (RAG)** based chatbot that enables users to interact with PDF documents through natural language queries. The system extracts text from uploaded PDFs, processes it into meaningful chunks, and generates embeddings using Google Gemini.

These embeddings are stored in a **FAISS vector database**, allowing efficient semantic search. When a user submits a query, the most relevant chunks are retrieved and passed to a Large Language Model (LLM), which generates accurate, context-aware responses strictly based on the document content.

The application is built with **Streamlit**, providing a simple and interactive interface for real-time document querying.

---
## 📌 Architecture

## 🚀 Features

* 📂 Upload and process PDF documents
* 🔍 Semantic search using vector embeddings
* 🧠 Context-aware question answering with Gemini LLM
* ⚡ Fast retrieval using FAISS vector store
* ✂️ Intelligent text chunking with overlap for better context retention
* 💬 Natural language querying interface
* 📊 Structured and well-explained responses
* 🚫 Strictly document-based answers (no hallucinated external info)

---

## 🧠 How It Works

The application follows a standard **RAG pipeline**:

1. **Document Upload**
   Users upload a PDF through the Streamlit interface.

2. **Text Extraction**
   The PDF is processed using `pdfplumber` to extract raw text.

3. **Text Chunking**
   The extracted text is split into smaller overlapping chunks using a recursive text splitter to preserve context.

4. **Embedding Generation**
   Each chunk is converted into vector embeddings using Google Gemini embedding models.

5. **Vector Storage (FAISS)**
   The embeddings are stored in a FAISS vector database for efficient similarity search.

6. **Query Processing**

   * User inputs a question
   * The system retrieves the most relevant chunks using semantic similarity (MMR search)

7. **Response Generation**
   The retrieved context is passed to the Gemini LLM along with a structured prompt to generate a final answer.

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Framework/UI:** Streamlit
* **LLM Integration:** Google Gemini (Generative AI)
* **Embeddings:** Gemini Embedding Model
* **Vector Database:** FAISS
* **Framework for LLM Orchestration:** LangChain
* **PDF Processing:** pdfplumber

---

## 🔮 Future Improvements

* 💾 Add conversational memory for multi-turn chat
* 📚 Support multiple PDF uploads and cross-document querying
* 📌 Display source citations for answers
* 🌐 Deploy the application on Streamlit Cloud or cloud platforms
* 🧠 Improve ranking with hybrid search (keyword + semantic)
* 🎯 Add user authentication and document management
* ⚡ Optimize performance for large documents

---

## 🤝 Contributing

Contributions are welcome!

If you'd like to improve this project:

1. Fork the repository
2. Create a new branch (`feature/your-feature-name`)
3. Commit your changes
4. Push to your branch
5. Open a Pull Request

Please ensure your code follows clean coding practices and includes proper documentation.

---

## 👩‍💻 Author

**Monica**

* Passionate about full-stack development, AI, and building practical applications
* Exploring LLMs, Generative AI, and automation tools

---

⭐ If you found this project useful, consider giving it a star!
