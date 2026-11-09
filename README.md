# MCP-Powered-Intelligent-Research-Assistant

# 📚 ResearchMate AI
### MCP-Powered Intelligent Research Assistant

ResearchMate AI is an AI-powered research assistant designed to simplify the process of exploring, understanding, and analysing academic research papers. It uses **Google Gemini API, Model Context Protocol (MCP), Python, and Streamlit** to help users interact with multiple research documents through an intelligent interface.

The application allows users to upload research papers, search for relevant information, generate summaries, compare different papers, identify potential research gaps, and ask questions across multiple documents.

## ✨ Features

- **PDF Document Management:** Upload and manage multiple research papers in PDF format.
- **Intelligent Document Search:** Search across research papers using TF-IDF and cosine similarity.
- **AI-Powered Summarisation:** Generate structured summaries covering research objectives, methodologies, models, datasets, results, limitations, and future directions.
- **Research Paper Comparison:** Compare two papers based on their architectures, methodologies, datasets, evaluation metrics, and findings.
- **Research Gap Identification:** Identify common limitations, unresolved problems, and potential research directions.
- **Multi-Paper Question Answering:** Ask natural-language questions and receive answers based on information retrieved from uploaded research papers.
- **Claim Verification:** Extract factual claims from summaries and check them against the original research documents.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Backend development |
| Google Gemini API | AI-powered analysis and generation |
| Model Context Protocol (MCP) | Communication between the AI application and research tools |
| Streamlit | Interactive web application |
| PyMuPDF | PDF text extraction |
| Scikit-learn | TF-IDF and cosine similarity |
| Asyncio | Asynchronous MCP communication |

## 🏗️ Architecture

The application follows an MCP-based architecture:

1. **Frontend:** Streamlit provides the interactive user interface.
2. **Backend:** Python manages application logic and user requests.
3. **MCP Client:** Communicates with the MCP server.
4. **MCP Server:** Provides tools for listing, reading, and searching research documents.
5. **Retrieval Engine:** TF-IDF and cosine similarity identify relevant document content.
6. **LLM Integration:** Google Gemini processes retrieved information and generates responses.

## ⚙️ How It Works

1. Users upload research papers in PDF format.
2. PyMuPDF extracts textual content from the documents.
3. The MCP server exposes document-processing and search tools.
4. The MCP client invokes the appropriate tools.
5. Relevant information is retrieved using TF-IDF-based search.
6. Retrieved information is passed to the Gemini API.
7. Gemini generates summaries, comparisons, research insights, and answers.

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/researchmate-ai.git
cd researchmate-ai
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Configure your Gemini API key securely using an environment variable:

```bash
GEMINI_API_KEY=your_api_key
```

Run the application:

```bash
streamlit run app.py
```

## 🎯 Project Objective

The primary objective of ResearchMate AI is to reduce the time and effort required to analyse academic literature. By combining MCP-based tool integration with large language models, the application provides an interactive platform for researchers and students to explore research papers and gain useful insights.

## 🔮 Future Enhancements

- Implement embedding-based semantic search.
- Integrate FAISS for vector-based document retrieval.
- Develop an advanced Retrieval-Augmented Generation (RAG) pipeline.
- Add source citations and page-level references.
- Support more document formats.
- Improve conversational memory and follow-up question handling.

## 👨‍💻 Author

**Somnath Sharma**

B.Tech – Computer Science and Engineering

Sikkim Manipal Institute of Technology

---

*ResearchMate AI – Making Research Smarter, Faster, and More Accessible.*
