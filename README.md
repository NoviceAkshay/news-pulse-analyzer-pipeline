# 📰 News Pulse Analyzer Pipeline

### AI-Powered Global News Intelligence System

---

## 🌍 Overview

**News Pulse Analyzer Pipeline** is an end-to-end data-driven application that collects, processes, and analyzes global news using AI and NLP techniques.

The system is designed as a **modular pipeline** that ingests news data, processes it through NLP techniques, and delivers structured insights via an interactive frontend.

This project demonstrates real-world concepts such as:

* Data ingestion pipelines
* API integration
* NLP preprocessing
* Backend–frontend communication
* Database design and querying
* Scalable application architecture

---

## 🚀 Key Features

* 🌐 Real-time news fetching using external APIs
* 🔍 Intelligent search with NLP-based normalization
* 🧠 Text preprocessing using SpaCy and NLTK
* 🗄 Structured data storage using PostgreSQL
* 🔐 User authentication system
* 📊 Interactive frontend using Streamlit
* ⚙️ Modular and extensible pipeline design

---

## 🧱 System Architecture

```
User (Streamlit UI)
        ↓
Frontend (Streamlit)
        ↓
FastAPI Backend (REST APIs)
        ↓
Data Processing Layer (NLP Pipeline)
        ↓
Database (PostgreSQL)
        ↓
External APIs (NewsAPI)
```

---

## 🔄 End-to-End Workflow

1. User interacts with the Streamlit interface
2. User logs in / registers
3. User enters a search query
4. Frontend sends request to FastAPI backend
5. Backend fetches news from NewsAPI
6. Data is cleaned and processed using NLP
7. Structured data is optionally stored in PostgreSQL
8. Processed results are returned to frontend
9. Streamlit displays formatted results

---

## 🛠 Tech Stack

### Backend

* FastAPI (Python)
* SQLAlchemy
* PostgreSQL

### Frontend

* Streamlit

### Data Processing

* SpaCy
* NLTK

### APIs

* NewsAPI

### Tools

* Git & GitHub
* PyCharm
* Virtual Environment (uv / venv)

---

## 🧠 Data Pipeline Breakdown

### 1. Data Ingestion

* Fetches news from NewsAPI
* Supports keyword-based queries
* Designed to extend to scraping/RSS feeds

---

### 2. Data Preprocessing (NLP Pipeline)

Includes:

* Lowercasing
* Punctuation removal
* Tokenization
* Stopword removal
* Lemmatization
* Query normalization

---

### 3. Data Structuring

* Stores structured news in PostgreSQL
* Enables efficient querying
* Schema-based storage (not raw dumping)

---

### 4. Output Generation

* Cleaned and relevant news results
* Filtered based on user query
* Extendable to classification, summarization, and insights

---

### 5. Visualization / Usage

* Displayed via Streamlit dashboard
* Can be extended to analytics dashboards or APIs

---

## ⚡ Backend Structure (FastAPI)

| File             | Description             |
| ---------------- | ----------------------- |
| main.py          | Entry point, API routes |
| database.py      | DB connection setup     |
| models.py        | Database schema         |
| auth.py          | Authentication logic    |
| text_cleaning.py | NLP preprocessing       |

---

## 🌐 Frontend (Streamlit)

Features:

* User login & registration
* Search interface
* Dynamic news display
* Session management

---

## 💾 Database Design

### Users Table

| Column     | Type      | Description  |
| ---------- | --------- | ------------ |
| id         | PK        | Unique ID    |
| username   | Unique    | Username     |
| email      | Unique    | Email        |
| created_at | Timestamp | Created time |

---

### News Table

| Column       | Type      | Description    |
| ------------ | --------- | -------------- |
| id           | PK        | Unique ID      |
| title        | Text      | News title     |
| description  | Text      | Summary        |
| url          | Text      | Article link   |
| published_at | Timestamp | Date           |
| source       | Text      | Source         |
| query_term   | Text      | Search keyword |

---

## 🧪 Example Flow

Input:
"GLoBAl TNDs"

Processed:
"global trends"

Output:
Relevant news articles retrieved and displayed

---

## 🚀 Running the Project

### Run Backend

```bash
uvicorn main:app --reload
```

### Run Frontend

```bash
streamlit run frontend/app.py
```

### Run Both Together

```bash
python run_all.py
```

---

## 📌 My Contribution

This project was originally developed as part of a team during an Infosys program.

Due to a shared repository setup, individual contributions are not fully reflected in the commit history.

In this version, I have:

* Re-structured and documented the pipeline
* Worked on data processing and NLP pipeline
* Implemented API integration logic
* Contributed to backend and debugging
* Improved overall system flow and usability

---

## 🔮 Future Enhancements

* Add LLM-based summarization (OpenAI / Claude)
* Implement real-time streaming pipeline
* Add sentiment analysis
* Deploy on cloud (AWS/Azure)
* Build analytics dashboard

---

## 📎 Proof of Work

This repository demonstrates:

* End-to-end pipeline development
* API integration
* NLP processing
* Full-stack application design

I can walk through:

* Architecture decisions
* Pipeline design
* Code implementation
* Scaling strategies

---

## 📚 References

* Streamlit Documentation
* FastAPI Documentation
* NewsAPI
* SpaCy Documentation
* NLTK Documentation

---

## 🤝 Final Note

This project reflects my ability to build real-world data-driven applications and my growing interest in scalable data pipelines and AI systems.
