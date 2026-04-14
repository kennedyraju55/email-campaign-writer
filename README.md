# 📧 Email Campaign Writer

[![Python 3.11+](https://img.shields.io/badge/Python-3.11%2B-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![MIT License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Gemma 4](https://img.shields.io/badge/Powered%20by-Gemma%204-orange?style=for-the-badge)](https://deepmind.google/technologies/gemma/)
[![Privacy First](https://img.shields.io/badge/Privacy-First-red?style=for-the-badge&logo=shield)](https://en.wikipedia.org/wiki/Privacy_by_design)
[![Ollama](https://img.shields.io/badge/Local%20LLM-Ollama-darkblue?style=for-the-badge)](https://ollama.ai)

> AI-powered email composition with Ollama, Gemma 4, and privacy preservation

## 🏗️ Architecture

```
Campaign Input → FastAPI Endpoints → Audience Analysis → Ollama + Gemma 4 Composer → Quality Checker → Campaign Ready
```

## ✨ Key Features

- Automatic professional email composition from keywords
- Tone adjustment (formal, casual, apologetic, persuasive)
- Subject line generation with optimization
- Multi-language email support
- Email template library with customization
- Grammar and spell-check integration
- Sentiment-aware response suggestions
- Privacy-first architecture using local Ollama
- Gemma 4 model for contextual understanding
- Campaign analytics and performance tracking

## 🚀 Quick Start

### Prerequisites
- Python 3.11 or higher
- Ollama installed and running (for local LLM)
- 4GB RAM minimum

### Installation

```bash
# Clone the repository
git clone https://github.com/kennedyraju55/email-campaign-writer.git
cd email-campaign-writer

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Running

```bash
# Start the application
python -m main
```

## 🔧 Tech Stack

| Component | Technology | Purpose |
|-----------|-----------|---------|
| **Backend Framework** | FastAPI | REST API endpoints |
| **LLM Runtime** | Ollama | Local model execution |
| **Model** | Gemma 4 | State-of-the-art language understanding |
| **Language** | Python 3.11+ | Core development language |
| **Processing** | NumPy/Pandas | Data manipulation |
| **Privacy** | Local Processing | No cloud dependencies |

## 📁 Project Structure

```
email-campaign-writer/
├── src/
│   ├── __init__.py
│   ├── core/
│   │   ├── models.py          # Data models
│   │   ├── config.py          # Configuration
│   │   └── exceptions.py      # Custom exceptions
│   ├── api/
│   │   ├── routes.py          # FastAPI endpoints
│   │   └── schemas.py         # Request/response schemas
│   ├── services/
│   │   ├── processor.py       # Main processing logic
│   │   └── ollama.py          # Ollama integration
│   └── utils/
│       ├── logger.py          # Logging setup
│       └── helpers.py         # Helper functions
├── tests/
│   ├── test_api.py
│   ├── test_services.py
│   └── conftest.py
├── requirements.txt           # Python dependencies
├── setup.py                   # Package configuration
├── README.md                  # This file
├── LICENSE                    # MIT License
└── .gitignore                 # Git ignore rules
```

## 📖 Usage Examples

```python
from src.services import processor

# Initialize processor
proc = processor.MainProcessor()

# Process your request
result = proc.process("your input")
print(result)
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Kennedy Raju** - *Creator & Maintainer*

- 🔗 [GitHub](https://github.com/kennedyraju55) - Follow for more projects
- 📝 [Dev.to](https://dev.to/kennedyraju55) - Technical articles and tutorials
- 💼 [LinkedIn](https://www.linkedin.com/in/nrk-raju-guthikonda-504066a8) - Professional network

## ⭐ Show Your Support

If you find this project helpful, please consider giving it a star! It helps others discover the project.

---

**Last Updated:** April 14, 2026
**Version:** 1.0.0
**Status:** Active Development
