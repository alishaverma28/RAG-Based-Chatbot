# 🧠 RAG-Based PDF Chatbot using Gemini & FAISS

🚀 **Live Application:**
👉 https://rag-based-pdf-chatbot-gemini.streamlit.app/

A **Retrieval-Augmented Generation (RAG)** powered chatbot that allows users to upload PDF documents and ask natural language questions, receiving **accurate, context-aware answers** grounded in the document content.

This project demonstrates an **end-to-end Generative AI pipeline** combining **LLMs, vector databases, embeddings, and a Streamlit UI**, built to production-ready standards.

---

## 🎯 Why This Project Stands Out

* ✅ Real-world **RAG architecture** implementation
* ✅ Uses **FAISS** for fast semantic vector search
* ✅ Powered by **Google Gemini LLM**
* ✅ Handles real **PDF documents**
* ✅ Secure API key handling using `.env`
* ✅ Live deployed Streamlit application
* ✅ Clean, modular, and interview-ready codebase

---

## 🧩 Application Workflow (RAG Pipeline)

1. **PDF Upload**
   User uploads a PDF document via the Streamlit sidebar

2. **Text Extraction**
   Text is extracted using a custom PDF extractor

3. **Chunking**
   Text is split into overlapping chunks using `RecursiveCharacterTextSplitter`

4. **Embedding Generation**
   Chunks are converted into embeddings using **HuggingFace MiniLM**

5. **Vector Storage**
   Embeddings are stored in a **FAISS vector database**

6. **Retrieval**
   Relevant document chunks are retrieved based on the user query

7. **Answer Generation**
   Retrieved context is passed to **Gemini LLM** to generate grounded responses

---

## 🛠️ Tech Stack

| Category               | Technology                            |
| ---------------------- | ------------------------------------- |
| Programming Language   | Python                                |
| UI Framework           | Streamlit                             |
| LLM                    | Google Gemini (gemini-2.5-flash-lite) |
| Vector Database        | FAISS                                 |
| Embeddings             | HuggingFace (all-MiniLM-L6-v2)        |
| Framework              | LangChain                             |
| PDF Processing         | PyPDF                                 |
| Environment Management | python-dotenv                         |

---

## 📁 Project Structure

```text
RAG-Based-Chatbot/
│
├── app.py                  # Main Streamlit application
├── pdfextractor.py         # Custom PDF text extraction logic
├── requirements.txt        # Project dependencies
├── .env                    # Environment variables (ignored by Git)
└── README.md               # Project documentation
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/RAG-Based-Chatbot.git
cd RAG-Based-Chatbot
```

### 2️⃣ Create & Activate Virtual Environment

```bash
python -m venv .venv

# Windows
.venv\Scripts\activate

# Linux / Mac
source .venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Configure Environment Variables

Create a `.env` file in the root directory:

```env
GOOGLE_API_KEY=your_google_gemini_api_key
```

⚠️ **Do NOT commit `.env` to GitHub**

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

## 🧪 How to Use

1. Upload a **PDF document**
2. Enter your question in the chat input
3. Receive **context-aware answers** from the chatbot
4. Continue the conversation with maintained chat history

---

## 💡 Use Cases

* 📄 Research paper Q&A
* 📚 Study material assistant
* 🧾 Policy and document analysis
* 🎓 Academic learning support
* 📑 Resume or report understanding

---

## 🔐 Security Best Practices

* API keys stored securely using environment variables
* `.env` file excluded via `.gitignore`
* No sensitive data logged or persisted

---

## 📌 Resume Bullet Points (ATS Optimized)

* Built a **Retrieval-Augmented Generation (RAG)** chatbot enabling PDF-based question answering using **Gemini LLM**.
* Implemented **semantic search** with **FAISS** and **HuggingFace MiniLM embeddings** for accurate document retrieval.
* Developed a complete **PDF processing pipeline** including text extraction, chunking, embedding, retrieval, and generation.
* Designed an interactive **Streamlit UI** with chat history and real-time responses.
* Applied secure credential management using **dotenv** and environment variables.
* Deployed a production-ready **GenAI application** demonstrating real-world LLM usage.

---

## 🚀 Future Enhancements

* Multi-PDF document support
* Source citation with page numbers
* Persistent chat memory
* User authentication
* Cloud-based vector storage

---

## 👩‍💻 Author

**Alisha Verma**

AI Engineer | Data Science & Analytics | GenAI Enthusiast
AWS Certified | Python | SQL | Cloud | AI

📫 *Open to AI Engineer*

---

⭐ *If you found this project useful, feel free to star the repository!*
