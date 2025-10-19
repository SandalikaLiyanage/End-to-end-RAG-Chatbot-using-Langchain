
#  RAG chatbot using LangChain

Built a RAG system using LangChain, integrating language models with document retrieval. (in api folder)

Developed a FastAPI backend to handle chat interactions and document management.(in api folder)

Created a user-friendly Streamlit frontend for seamless interaction with our RAG chatbot. (in app folder)

## 🗂️ Project Structure

| File | Description |
|------|--------------|
| `main.py` | FastAPI backend with REST endpoints |
| `db_utils.py` | SQLite database for chat logs and document metadata |
| `chroma_utils.py` | Vector database utilities for semantic search |
| `langchain_utils.py` | LangChain RAG pipeline logic |

## Getting Started

1. ## Clone the Repository

```bash
git clone https://github.com/insighture/dspy-rag-bot.git
cd dspy-rag-bot
```

2. ## Set Up Environment Variables
*Create a .env file:*
```bash
OPENAI_API_KEY=your_openai_key
```

3. ## Create a virtual environment
```bash
python -m venv venv
```

4. ## Activate the virtual environment
*On Windows:*
```bash
venv\Scripts\activate
```

*On macOS/Linux:*
```bash
source venv/bin/activate
```

5. ## Initialize uv (creates pyproject.toml)
```bash
uv init
```

6. ## Add dependencies
```bash
uv add langchain langchain-openai langchain-core langchain_community \
       docx2txt pypdf langchain_chroma python-multipart streamlit
```

7. ## Run the App
*Backend:*
```bash
cd api
uvicorn main:app --reload
```
*Frontend:*
```bash
cd app
streamlit run streamlit_app.py
```





