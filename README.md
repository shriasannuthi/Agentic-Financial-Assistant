# Financial RAG Assistant

An Agentic AI-powered financial assistant that analyzes customer documents, retrieves relevant information using Retrieval-Augmented Generation (RAG), performs web search when required, and generates comprehensive financial reports.

---

## Overview

Financial RAG Assistant combines multiple AI agents to understand customer requests, retrieve information from uploaded financial documents, search the web for current financial information when necessary, and generate structured reports.

The application leverages **CrewAI**, **LangChain**, and **OpenAI** models to orchestrate specialized agents for intelligent financial analysis.

---

## Features

- PDF document analysis
- Multi-agent AI workflow
- Retrieval-Augmented Generation (RAG)
- Intelligent web search
- Automated financial report generation
- Email-ready report output
- Natural language financial queries
- Context-aware document retrieval

---

## Architecture

![Architecture](architecture.png)

The system consists of multiple specialized AI agents:

- Router Agent
- Retriever Agent
- Report Generator Agent
- Search Agent

These agents collaborate to determine whether a query should be answered using uploaded documents, web search, or general LLM reasoning.

---

## Workflow

![Workflow](workflow.png)

1. User submits a question.
2. Financial documents are uploaded.
3. Router Agent determines the appropriate execution path.
4. Retriever Agent extracts relevant information using RAG.
5. Search Agent gathers current financial information when required.
6. Report Generator compiles the final response.
7. Report is returned to the user.

---

## Tech Stack

### AI Frameworks

- CrewAI
- LangChain
- OpenAI GPT-4o Mini

### Backend

- Python
- FastAPI

### Document Processing

- PyPDF
- PDFSearchTool

### Search

- Google Serper API

### Other Libraries

- python-dotenv
- Groq
- DuckDuckGo Search
- PhiData

---

## Project Structure

```
.
├── app.py
├── agenticRAG.py
├── architecture.png
├── workflow.png
├── requirements.txt
├── Report.pdf
└── Demo Videos
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/shriasannuthi/Financial-RAG-Assistant.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Configure your environment variables

```env
OPENAI_API_KEY=
SERPER_API_KEY=
```

Run the application

```bash
python app.py
```

---

## AI Agents

### Router Agent

Determines whether the query should use:

- RAG
- Web Search
- LLM Generation

---

### Retriever Agent

Extracts relevant financial information from uploaded PDF documents without modifying factual content.

---

### Search Agent

Retrieves current financial information including:

- Interest rates
- Market trends
- Banking products
- Company information

---

### Report Generator Agent

Compiles retrieved information into a structured financial report tailored to the user's request.

---

## Example Use Cases

- Loan eligibility analysis
- Customer financial profiling
- Financial document summarization
- Banking customer support
- Financial report generation
- Market information retrieval

---

## Future Improvements

- Multi-document indexing
- Vector database integration
- Streamlit frontend
- Authentication
- OCR support
- Voice interface
- Multi-language support
- Cloud deployment

---

## Author

**Shria Sannuthi**

Software Engineer | Generative AI | Agentic AI | RAG | LLM Applications

---

## 📄 License

MIT License
