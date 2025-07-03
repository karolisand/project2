# project2

## Description

**project2** is an AI-powered chatbot web application built with Streamlit. It leverages OpenAI's GPT models and integrates web search (DuckDuckGo) and PostgreSQL database access. The assistant can answer questions using up-to-date web information and database queries, always citing its sources.

## Features

- 🤖 **AI Chatbot**: Chat with an OpenAI GPT model in your browser
- 🔎 **Web Search**: Get real-time answers using DuckDuckGo search
- 🗄️ **Database Access**: Query a PostgreSQL movie database (1000+ films, customers, rentals)
- 🧠 **Intelligent Routing**: Automatically uses web search or database as needed
- 📚 **Source Citations**: All web-based answers include references
- 🧩 **Extensible**: Easily add new tools or data sources

## Libraries Used

- [streamlit](https://streamlit.io/) - Web app framework
- [openai-agents](https://pypi.org/project/openai-agents/) - Agent orchestration
- [duckduckgo-search](https://pypi.org/project/duckduckgo-search/) - Web search API
- [python-dotenv](https://pypi.org/project/python-dotenv/) - Environment variable management

## Getting Started

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd project2
```

### 2. Install dependencies

You need Python 3.12+ installed. Install dependencies using [uv](https://github.com/astral-sh/uv) (recommended) or pip:

```bash
# Using uv (recommended)
uv pip install -r requirements.txt
# Or using pip
pip install -r requirements.txt
```

Or, if using `pyproject.toml`:

```bash
pip install .
```

### 3. Add your OpenAI API key

Create a `.env` file in the project root with the following content:

```env
OPENAI_API_KEY=your_openai_api_key_here
```

You can get your OpenAI API key from [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys).

### 4. Launch the application

```bash
streamlit run main.py
```

The app will open in your browser. Start chatting!

## Usage

1. Type your message in the chat input box.
2. Press Enter to send.
3. The assistant will respond, using web search or database as needed.
4. Use the sidebar to clear chat history or view instructions.

## Environment Variables

- `OPENAI_API_KEY` (required): Your OpenAI API key for GPT model access.

## License

MIT License. See [LICENSE](LICENSE) for details.