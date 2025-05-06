# Cairo-Tourism-Search-Chatbot-RAG-Based-
<!-- Uploading "finalproject2RAG (online-video-cutter.com).mp4"... -->
This project is a Retrieval-Augmented Generation (RAG) chatbot designed to help users explore tourist attractions in **Cairo, Egypt** using **Arabic** queries. It combines **semantic search**, **language embeddings**, and a **Gradio** interface to create an intelligent tourism assistant.

---

## 📌 Features

- ✅ Arabic-language support using multilingual embeddings  
- ✅ Real-time semantic search with FAISS  
- ✅ Intuitive chatbot-style interface with Gradio  
- ✅ Structured guide scraped from a popular Egyptian travel blog  
- ✅ Efficient search over dense vector representations

---

## 🛠️ Tech Stack

| Component         | Tool/Library                          |
|------------------|----------------------------------------|
| Web Scraping      | `requests`, `BeautifulSoup`            |
| Embeddings        | `intfloat/multilingual-e5-large` (Sentence Transformers) |
| Semantic Search   | `FAISS` (IndexFlatIP for cosine similarity) |
| Interface         | `Gradio`                              |
| Dataset Handling  | `Hugging Face Datasets`               |

---

## 🧠 How It Works

1. **Web Scraping**  
   Scrapes structured Arabic content about Cairo tourism from *PropertyFinder Egypt*.

2. **Data Chunking**  
   Uses regex to split the text into semantically meaningful chunks.

3. **Text Embedding**  
   Uses `multilingual-e5-large` to convert text chunks into high-dimensional vectors.

4. **FAISS Search**  
   Creates an efficient vector index and retrieves top-k similar chunks for each query.

5. **Chatbot Interface**  
   A Gradio app allows users to input Arabic queries and receive relevant tourist info.

---

## 🚀 Getting Started

### 1. Clone the Repo
```bash
git clone https://github.com/yourusername/cairo-tourism-chatbot.git
cd cairo-tourism-chatbot
