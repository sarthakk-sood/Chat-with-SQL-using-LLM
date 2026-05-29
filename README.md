# 🚀 Chat with SQL using LLM

[![Live Demo - Try it Now!](https://img.shields.io/badge/Live%20Demo-Streamlit-brightgreen?logo=streamlit&labelColor=black)](https://chat-with-sql-using-llm-hxaeb27juug2h2uuh6x6pb.streamlit.app/)

An interactive Streamlit application that lets you chat with SQLite and MySQL databases using natural language. Powered by [LangChain](https://www.langchain.com/), Groq's blazing-fast Llama 3 LLMs, and AI-driven SQL agents.

---

## ✨ Features

- **Natural Language to SQL:** Ask questions in plain English—AI writes and executes the SQL queries for you.
- **Works with Both SQLite & MySQL:** Query the included demo SQLite (`student.db`) or connect to your own MySQL server via the UI.
- **High-Speed / Low-Latency:** Leverages Groq's `llama-3-70b` for lightning-fast responses.
- **Conversational Memory:** Maintains chat context so you can ask follow-up questions.
- **Schema-Aware Agent:** Automatically inspects your DB schema to generate safe and accurate queries.
- **No Local Setup Required:** Try it instantly with the [Live Demo](https://chat-with-sql-using-llm-hxaeb27juug2h2uuh6x6pb.streamlit.app/).

---

## 🖥️ Live Demo

👉 **[Launch the App Now on Streamlit Cloud! 🚀](https://chat-with-sql-using-llm-hxaeb27juug2h2uuh6x6pb.streamlit.app/)**

> No setup needed! Try chatting with the sample database immediately.

---

## 🛠️ Local Installation

**Prerequisites**
- Python 3.10+
- A [Groq API Key](https://console.groq.com/keys) (free signup)

**Step-by-step:**

1. **Clone this repo**
    ```bash
    git clone https://github.com/sarthakk-sood/Chat-with-SQL-using-LLM.git
    cd Chat-with-SQL-using-LLM
    ```
2. **(Recommended) Create and activate a virtual environment**
    ```bash
    python -m venv venv
    source venv/bin/activate # (or `venv\Scripts\activate` on Windows)
    ```
3. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    # OR if not present:
    pip install streamlit langchain langchain-community langchain-groq sqlalchemy python-dotenv mysql-connector-python
    ```
4. **Add your Groq API key**
    - Create a `.env` file in the project root:
      ```
      GROQ_API_KEY="gsk_your_actual_api_key_here"
      ```

---

## ▶️ Usage

1. **Start the Streamlit app:**
    ```bash
    streamlit run app.py
    ```

2. **Open your browser at the printed URL** (usually [http://localhost:8501](http://localhost:8501)).

3. **Connect to a database:**
    - Choose between the local SQLite demo or your own MySQL.
    - For MySQL, enter your host/user/password.

4. **Ask questions!**
    - Example: "Show all students in Data Science."
    - Example: "Which student scored highest?"

---

## 🏗️ Built With

- [Streamlit](https://streamlit.io/) — Web UI
- [LangChain](https://www.langchain.com/) — LLM orchestration & SQL agent
- [Groq](https://groq.com/) — Llama 3 LLM backend
- [SQLAlchemy](https://www.sqlalchemy.org/) — SQL database toolkit

---

