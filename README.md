# Memori

A fork of [MemoriLabs/Memori](https://github.com/MemoriLabs/Memori) — an AI-powered memory and knowledge management system.

## Features

- 🧠 Persistent memory across conversations
- 🔍 Semantic search over stored memories
- 🔗 Integration with popular LLM providers
- 🐳 Docker support for easy deployment
- 🔒 Secure API key management

## Quick Start

### Prerequisites

- Python 3.11+
- Docker & Docker Compose (optional)
- An OpenAI API key (or compatible provider)

### Local Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/memori.git
   cd memori
   ```

2. **Create a virtual environment**

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Configure environment**

   ```bash
   cp .env.example .env
   # Edit .env with your API keys and settings
   ```

5. **Run the application**

   ```bash
   python -m memori
   ```

### Docker Setup

```bash
docker compose up -d
```

The API will be available at `http://localhost:8000`.

## Configuration

See [`.env.example`](.env.example) for all available configuration options.

| Variable | Description | Default |
|---|---|---|
| `OPENAI_API_KEY` | Your OpenAI API key | required |
| `DATABASE_URL` | Database connection string | `sqlite:///memori.db` |
| `LOG_LEVEL` | Logging verbosity | `INFO` |

## API Reference

Once running, visit `http://localhost:8000/docs` for the interactive API documentation.

## Contributing

We welcome contributions! Please check out:

- [Bug Reports](.github/ISSUE_TEMPLATE/bug_report.yml)
- [Feature Requests](.github/ISSUE_TEMPLATE/feature_request.yml)
- [Pull Request Template](.github/pull_request_template.md)

### Development

```bash
# Install dev dependencies
pip install -r requirements-dev.txt

# Run tests
pytest

# Lint
ruff check .
```

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Original project: [MemoriLabs/Memori](https://github.com/MemoriLabs/Memori)
