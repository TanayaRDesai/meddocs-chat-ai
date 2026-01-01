# 🏥 MediChat Pro

**MediChat Pro** is an intelligent medical document chatbot that allows users to upload medical PDF documents and interact with them using natural language. The app uses **Streamlit** for the UI, **FAISS** for vector search, and **LangChain** with **Euri AI** for generating accurate, context-aware answers.

---

## 🚀 Features

- 📄 Upload multiple medical PDF documents
- 🔍 Automatic text extraction and intelligent chunking
- 🧠 Semantic search using FAISS vector store
- 💬 Chat interface to ask questions from uploaded documents
- ⏱️ Chat history with timestamps
- 🎨 Clean, user-friendly Streamlit UI

---

## 🛠️ Tech Stack

- **Frontend / UI**: Streamlit
- **LLM Integration**: Euri AI
- **Framework**: LangChain
- **Vector Database**: FAISS
- **PDF Processing**: PyPDF
- **Embeddings**: Sentence Transformers
- **Language**: Python

---

## 📂 Project Structure

```
MedChat-Pro/
│
├── main.py                  # Main Streamlit application
├── requirements.txt         # Project dependencies
├── app/
│   ├── config.py            # API keys and configuration
│   ├── chat_utils.py        # Chat model setup and query logic
│   ├── pdf_utils.py         # PDF text extraction utilities
│   ├── vectorstore_utils.py # FAISS index creation & retrieval
│   └── ui.py                # UI helper components
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/medichat-pro.git
cd medichat-pro
```

### 2️⃣ Create Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Configure API Key

Add your **Euri AI API key** in `app/config.py`:

```python
EURI_API_KEY = "your_api_key_here"
```

---

## ▶️ Running the Application

```bash
streamlit run main.py
```

The app will open in your browser at:

```
http://localhost:8501
```

---

## 🧪 How It Works

1. Upload one or more **medical PDF documents**
2. Click **Process Documents**
3. PDFs are:
   - Converted to text
   - Split into chunks
   - Stored in FAISS vector index
4. Ask questions in the chat
5. Relevant document context is retrieved and sent to the LLM
6. AI responds based only on uploaded documents

---

## ⚠️ Important Notes

- This tool is for **information assistance only**
- It does **not replace professional medical advice**
- If an answer is not found in documents, the bot clearly states it

---

## 📌 Future Enhancements

- 🔐 User authentication
- 📊 Document summary view
- 🧾 Support for non-PDF formats
- ☁️ Cloud deployment
- 🩺 Medical entity highlighting
---

## 👩‍💻 Author

**Tanaya Desai**  
AI & Python Enthusiast

---

⭐ If you like this project, don’t forget to star the repository!

