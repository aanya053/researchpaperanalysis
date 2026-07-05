# 📚 AI Research Paper Intelligence System

An AI-powered research paper search engine that enables semantic retrieval over ArXiv Machine Learning papers using Sentence Transformers and FAISS. The system combines semantic search, keyword-based retrieval, AI-generated summaries, and keyword extraction to help users discover relevant research papers efficiently.

---

## 🚀 Features

- 🔍 Hybrid Search (Semantic Search + TF-IDF)
- 📖 Semantic Retrieval using Sentence Transformers
- ⚡ Fast Vector Search with FAISS
- 🤖 AI-generated Paper Summaries using DistilBART
- 🏷️ Automatic Keyword Extraction using KeyBERT
- 📄 Similar Paper Recommendations
- ⭐ Save Favorite Papers
- 📥 Export Search Results as CSV
- 📊 Similarity Score for each paper
- 🎨 Interactive Streamlit Web Interface

---

## 🛠️ Tech Stack

- Python
- Streamlit
- Sentence Transformers
- FAISS
- Hugging Face Transformers
- KeyBERT
- Scikit-learn
- Pandas
- NumPy
- Hugging Face Datasets

---

## 📂 Project Structure

```
AI_RESEARCHPAPER
│
├── data/
│   ├── cleaned_arxiv_papers.csv
│   ├── paper_faiss.index
│   └── arxiv_embeddings.npy
│
├── src/
│   ├── app.py
│   ├── build_index.py
│   ├── data_prep.py
│   ├── search_engine.py
│   └── config.py
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 📊 Workflow

1. Download and preprocess the ArXiv Machine Learning dataset.
2. Generate sentence embeddings using **all-MiniLM-L6-v2**.
3. Build a FAISS vector index for semantic retrieval.
4. Build a TF-IDF index for keyword-based retrieval.
5. Perform hybrid search by combining semantic similarity and keyword relevance.
6. Generate AI summaries using DistilBART.
7. Extract important keywords using KeyBERT.
8. Display ranked results through a Streamlit interface.

---

## 🧠 Models Used

### Embedding Model
- sentence-transformers/all-MiniLM-L6-v2

### Summarization Model
- sshleifer/distilbart-cnn-12-6

### Keyword Extraction
- KeyBERT

---

## 📦 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/AI_RESEARCHPAPER.git
```

Move into the project directory

```bash
cd AI_RESEARCHPAPER
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the environment

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

### Step 1

Prepare the dataset

```bash
python src/data_prep.py
```

### Step 2

Generate embeddings and build the FAISS index

```bash
python src/build_index.py
```

### Step 3

Launch the Streamlit application

```bash
streamlit run src/app.py
```

---

## 📈 Future Improvements

- Cross-Encoder Re-ranking
- Research Paper Recommendation System
- Citation Network Visualization
- Multi-document Question Answering
- PDF Upload and Search
- LLM-powered Research Assistant
- Voice-based Paper Search

---

## 📚 Dataset

The project uses the **CShorten/ML-ArXiv-Papers** dataset available on Hugging Face.

---

## 👩‍💻 Author

**Aanya Mahajan**

Computer Science Engineering Student

Interested in Artificial Intelligence, Machine Learning, NLP, and Full-Stack Development.

---

## 📄 License

This project is intended for educational and research purposes.
