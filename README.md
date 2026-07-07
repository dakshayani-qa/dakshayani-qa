### Hi, I'm Dakshayani 👋

QA Automation Engineer passionate about building AI-powered testing tools.

- 🔭 Currently building: **TestPilot AI** — an AI agent pipeline that generates
  QA test cases (positive/negative/edge/regression) from requirement documents
  using local LLMs
- 🛠️ Skills: Python, Test Automation, AI Agents, Ollama, Streamlit, Selenium, SQL
- 📫 Reach me: dakshu.tech26@gmail.com | [LinkedIn URL]

### Featured Project
**[TestPilot AI](https://github.com/yourusername/testpilot-ai-test-case-generator)**
AI-powered test case generator that reads requirement docs (PDF, Word, Excel,
CSV, Text) and auto-generates categorized test cases with regression tagging —
built entirely on free, open-source tools, runs fully local.
# 🤖 AI Test Case Generator using Llama 3.2, Ollama & RAG

## 📌 Project Overview

The **AI Test Case Generator** is a Generative AI-powered application that automatically generates software test cases from requirement documents such as BRD, FRD, SRS, PDF, and DOCX files.

The application leverages **Retrieval-Augmented Generation (RAG)** with **Llama 3.2** running locally through **Ollama** to understand requirements and generate comprehensive test scenarios. Document embeddings are stored in **ChromaDB**, enabling semantic search and context-aware test case generation.

This solution helps QA teams significantly reduce manual effort while improving test coverage and consistency.

---

## 🚀 Features

- Upload PDF and DOCX requirement documents
- Automatic document ingestion and preprocessing
- Intelligent text chunking
- Vector embedding storage using ChromaDB
- Semantic search using Retrieval-Augmented Generation (RAG)
- AI-powered test case generation using Llama 3.2
- Generates:
  - Positive Test Cases
  - Negative Test Cases
  - Boundary Value Test Cases
  - Validation Test Cases
  - Error Handling Test Cases
  - Exception Test Cases
- Interactive Streamlit web interface
- Local LLM execution using Ollama (No external API dependency)

---

# 🏗️ Solution Architecture

```
            Requirement Document
                 (PDF/DOCX)
                      │
                      ▼
             Document Ingestion
                      │
                      ▼
              Text Extraction
                      │
                      ▼
              Intelligent Chunking
                      │
                      ▼
         ChromaDB Vector Database
                      │
                      ▼
         Semantic Similarity Search
                      │
                      ▼
      Retrieval Augmented Generation
                      │
                      ▼
         Ollama + Llama 3.2 LLM
                      │
                      ▼
      AI Generated Software Test Cases
```

---

# ⚙️ Technology Stack

| Category | Technologies |
|----------|--------------|
| Programming | Python |
| LLM | Llama 3.2 |
| LLM Runtime | Ollama |
| Vector Database | ChromaDB |
| AI Architecture | Retrieval-Augmented Generation (RAG) |
| UI | Streamlit |
| Document Processing | PyPDF2, python-docx |
| Embeddings | Sentence Transformers |
| Prompt Engineering | Custom Prompts |

---

# 📂 Project Structure

```
AI-Test-Case-Generator/

│
├── app.py
├── requirements.txt
├── README.md
│
├── agents/
│   ├── ingestion.py
│   ├── retriever.py
│   ├── test_case_generator.py
│
├── utils/
│   ├── chunking.py
│   ├── embedding.py
│   ├── parser.py
│
├── chroma_db/
│
├── uploads/
│
└── generated_testcases/
```

---

# 🔄 Workflow

## Step 1 – Upload Requirement Document

Users upload a requirement document in PDF or DOCX format through the Streamlit interface.

---

## Step 2 – Document Ingestion

The system reads the uploaded document and extracts textual content.

---

## Step 3 – Intelligent Chunking

The extracted text is divided into smaller semantic chunks to improve retrieval accuracy.

---

## Step 4 – Embedding Generation

Each chunk is converted into vector embeddings using an embedding model.

---

## Step 5 – Store in ChromaDB

Generated embeddings are stored in ChromaDB Vector Database for efficient similarity search.

---

## Step 6 – Semantic Retrieval

When generating test cases, relevant requirement chunks are retrieved using semantic similarity search.

---

## Step 7 – AI Test Case Generation

The retrieved context is combined with optimized prompts and passed to **Llama 3.2** through Ollama.

The LLM generates comprehensive software test cases.

---

## Step 8 – Display Results

Generated test cases are displayed in the Streamlit application.

---
# ▶️ Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/AI-Test-Case-Generator.git
```

---

## Navigate to Project

```bash
cd AI-Test-Case-Generator
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Install Ollama

Download and install Ollama.

Pull the Llama 3.2 model:

```bash
ollama pull llama3.2
```

---

## Run Application

```bash
streamlit run app.py
```

---

# 📋 Types of Test Cases Generated

- Functional Test Cases
- Positive Test Cases
- Negative Test Cases
- Boundary Value Analysis
- Validation Testing
- Error Handling
- Exception Testing

---

# 💡 Key Features

- AI-powered Requirement Analysis
- Prompt Engineering
- Local LLM Inference
- Vector Database Search
- Retrieval-Augmented Generation
- Semantic Search
- Automated Test Design
- Interactive User Interface

- # 📈 Business Benefits

- Reduces manual test design effort
- Improves requirement coverage
- Generates consistent test cases
- Accelerates QA activities
- Supports AI-assisted software testing
- Enhances productivity using Generative AI

---

# 🎯 Future Enhancements

- Export test cases to Excel
- Export to Azure DevOps
- Jira integration
- Test case prioritization
- AI-generated automation scripts
- Risk-based testing recommendations
- Multi-model LLM support
- Cloud deployment

---

# 👩‍💻 Author

**Dakshayani V**

AI QA Engineer | Test Automation Engineer | Generative AI Enthusiast

**Skills**

- Python
- Playwright
- Selenium
- Generative AI
- Prompt Engineering
- Ollama
- Llama 3.2
- ChromaDB
- Retrieval-Augmented Generation (RAG)
- Streamlit

---

# ⭐ If you found this project useful, consider giving it a Star!
