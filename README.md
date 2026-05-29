# ðŸ¦œ LangChain: Chat with SQL DB

An interactive Streamlit web application that enables users to chat with their SQL databases using natural language. Powered by LangChain, Groq's high-speed LLMs (Llama 3), and an AI-driven SQL Agent, this tool converts your conversational questions into executable SQL queries, runs them against your database, and returns the answers in plain English.

## âœ¨ Features
- **Natural Language to SQL**: Ask questions in plain English and let the AI write and execute the SQL queries.
- **Local & Remote Database Support**: 
  - Effortlessly query the included local SQLite database (`student.db`).
  - Dynamically connect to a remote MySQL database by providing host, user, and password via the UI.
- **High-Speed AI**: Utilizes Groq's blazing-fast inference with the `llama-3.3-70b-versatile` model.
- **Chat History**: Maintains a conversational memory during your session so you can ask follow-up questions.
- **Transparent Execution**: The LangChain SQL Agent dynamically explores table schemas and structures before formulating queries to ensure accurate results.

## ðŸ› ï¸  Prerequisites
- Python 3.10+
- A valid [Groq API Key](https://console.groq.com/keys)

## ðŸš€ Installation & Setup

1. **Clone the repository** (if you haven't already):
   ```bash
   git clone https://github.com/YOUR_USERNAME/ChatWithSQL-App.git
   cd ChatWithSQL-App
   ```

2. **Set up a virtual environment** (Recommended):
   ```bash
   conda create -p langenv python=3.11 -y
   conda activate ./langenv
   ```

3. **Install dependencies**:
   Make sure you have the required libraries installed. You can install them via pip:
   ```bash
   pip install streamlit langchain langchain-community langchain-groq sqlalchemy python-dotenv mysql-connector-python
   ```

4. **Configure your Environment Variables**:
   Create a `.env` file in the root of the project directory and add your Groq API key:
   ```env
   GROQ_API_KEY="gsk_your_actual_api_key_here"
   ```

## ðŸ’» Usage

Run the Streamlit application from your terminal:

```bash
streamlit run app.py
```

1. Open the local URL provided by Streamlit (usually `http://localhost:8501`).
2. Select your database source from the sidebar (Local SQLite or MySQL).
3. Start asking questions like *"Which student has the highest marks?"* or *"How many students are in the Data Science course?"*

## ðŸ› ï¸  Built With
- [Streamlit](https://streamlit.io/) - Front-end web framework
- [LangChain](https://www.langchain.com/) - LLM orchestration and Agent toolkit
- [Groq](https://groq.com/) - Lightning-fast inference engine
- [SQLAlchemy](https://www.sqlalchemy.org/) - Database connection modeling