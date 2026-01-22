
# Resume-to-Job Matcher and Cold Email Generator 💼🤖

This is an advanced **AI-powered resume-job matching platform** designed to help job seekers instantly tailor their resumes to job postings, generate cold outreach emails, and get personalized project suggestions. Built using **LLMs**, **vector databases**, and **resume analysis**, this tool replicates the real-world logic of how recruiters screen and score resumes using ATS systems.

---

## 🚀 Overview

Users can upload multiple PDF resumes and provide a job listing URL. The tool:
- Scrapes and cleans the job description
- Extracts structured job requirements (skills, experience, role)
- Matches resumes using both **semantic** and **keyword-based** logic
- Scores each resume on a custom-built **ATS simulation engine**
- Recommends resume improvements (missing skills)
- Suggests domain-specific **project ideas** based on required skills
- Generates a **personalized cold email** for the role

---

## 🧠 Key Features

- 🔹 Gemini-powered LLM reasoning (LLama3 / Gemini Flash)
- 🔹 Cold email generator using resume + job description + skills
- 🔹 ATS-like scoring engine (semantic + keyword + project relevance)
- 🔹 Resume skill gap detection
- 🔹 Project recommendations based on skill-job alignment
- 🔹 Modular architecture with clean separation of concerns

---

## 📋 Required CSV Format

Before using the tool, users must create a **CSV file** (`suman_projects.csv`) containing project metadata:

### 🔹 Format:
| Project Name         | Skills Used                                      |
|----------------------|--------------------------------------------------|
| Smart News Summarizer| Python, LLM, LangChain, HuggingFace, Streamlit  |
| AI Resume Parser     | NLP, spaCy, Resume Parsing, PDF Extraction      |

This CSV powers the **project similarity and recommendation engine** that maps job-required skills to your past work.

---

## 🧪 How It Works

1. **Input**: Upload resumes + job link
2. **Scraping & Parsing**: Job listing is scraped and structured using LLM
3. **Resume Matching**: All resumes are scored on multiple ATS-like metrics:
   - Semantic relevance (LLM embeddings)
   - Keyword match
   - Role alignment
   - Experience fit
   - Project relevance
4. **Best Match**: Top-scoring resume is selected
5. **Suggestions**: Missing skills and project ideas are presented
6. **Cold Email**: Personalized recruiter email is generated
7. **Chatbot**: Personal Chatbot on the same platform

---

## 🛠️ Setup Instructions

### 1. Clone the repo
```bash
git clone https://github.com/your-username/resume-job-matcher.git
cd resume-job-matcher
```

### 2. Set up a virtual environment and install dependencies
```bash
pip install -r requirements.txt
```

### 3. Create a `.env` file with your keys
```
GEMINI_API_KEY=your_gemini_key
GROQ_API_KEY=your_grok_cloud_key
```

---

## ✅ Run the App

```bash
streamlit run main.py
```

Open your browser at `http://localhost:8501` to use the app.

---

## 📦 Key Dependencies

- `streamlit`
- `langchain`
- `faiss-cpu`
- `langchain-google-genai`
- `sklearn`
- `python-dotenv`
- `pandas`

---

## 📚 Learn More

- [Gemini API](https://ai.google.dev)
- [LangChain](https://www.langchain.com)
- [FAISS Vector DB](https://github.com/facebookresearch/faiss)

---

## 📌 Author

Built by [Surendhar Bandari](https://github.com/Surenbandari) — making job applications smarter with AI.

---

## 📜 License

Apache License Version 2.0
