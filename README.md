# LangChain MCP Demo

This project demonstrates how to integrate GitHub MCP (Model Context Protocol) server with LangChain workflows.

## Features

- Integration of GitHub MCP server with LangChain tools
- Example workflows for repository information retrieval
- Type-annotated, clean code following best practices

## Setup

1. Clone this repository
2. Install dependencies with Poetry:
   ```bash
   cd langchain-mcp-demo
   poetry install
   ```
3. Set up environment variables:
   ```bash
   cp .env.example .env
   # Edit .env with your GitHub token
   ```

## Usage

Run the demo:

```bash
poetry run python -m langchain_mcp_demo.run_demo
```

## Project Structure

```
langchain-mcp-demo/
├── langchain_mcp_demo/
│   ├── __init__.py
│   ├── mcp_client.py       # GitHub MCP client wrapper
│   ├── mcp_tools.py        # LangChain tools using MCP
│   ├── chains.py           # LangChain chains using MCP tools
│   └── run_demo.py         # Demo script
├── tests/
│   ├── __init__.py
│   ├── test_mcp_client.py
│   └── test_chains.py
├── .env.example
├── pyproject.toml
├── poetry.lock
└── README.md
```

## Development

This project uses:
- Poetry for dependency management
- Black and isort for formatting
- Flake8 for linting
- Pytest for testing

## License

MIT