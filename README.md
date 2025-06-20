# AI Voice Assistant

[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An advanced AI-powered voice assistant that combines speech-to-text and text-to-speech capabilities with intelligent tool integration for seamless digital interactions.

## Overview

This AI Voice Assistant provides natural conversational experiences through voice interaction while offering powerful integrations with Google services, web search, and personal knowledge management. The assistant can understand spoken commands, process requests using various tools, and respond with synthesized speech.

## Key Features

### Core Capabilities
- **Speech Recognition**: Real-time speech-to-text conversion using Deepgram API
- **Voice Synthesis**: Natural text-to-speech responses
- **Conversational AI**: Powered by advanced language models (Llama3, Gemini)
- **Multi-tool Integration**: Seamless access to productivity and information tools

### Integrated Tools

| Tool | Description | Functionality |
|------|-------------|---------------|
| **CalendarTool** | Google Calendar integration | Schedule events with date, time, and descriptions |
| **AddContactTool** | Contact management | Add new contacts to Google Contacts |
| **FetchContactTool** | Contact retrieval | Search and retrieve contact information |
| **EmailingTool** | Gmail integration | Compose and send emails |
| **SearchWebTool** | Web search | Access real-time web information via Tavily API |
| **KnowledgeBaseTool** | Personal knowledge base | Query documents from `/files` directory |

## Installation

### Prerequisites

- Python 3.9 or higher
- Google Cloud Platform account with API access
- Required API keys (see configuration section)

### Quick Start

1. **Clone the repository**
```bash
git clone https://github.com/danieladdisonorg/AI-Voice-Assitant.git
```

2. **Navigate to project directory**
```bash
cd AI-Voice-Assitant
```

3. **Create virtual environment**
```bash
python -m venv venv
```

4. **Activate virtual environment**
```bash
source venv/bin/activate
```

5. **Install dependencies**
```bash
pip install -r requirements.txt
```

## Configuration

### Environment Variables

Create a `.env` file in the project root:

```env
# Google Services
GOOGLE_API_KEY=your_google_api_key
GEMINI_API_KEY=your_gemini_api_key

# Speech Processing
DEEPGRAM_API_KEY=your_deepgram_api_key

# Web Search
TAVILY_API_KEY=your_tavily_api_key

# Language Model
GROQ_API_KEY=your_groq_api_key
```

### Google API Setup

1. Visit the [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select an existing one
3. Enable the following APIs:
   - Google Calendar API
   - Google Contacts API
   - Gmail API
4. Create service account credentials
5. Download the credentials JSON file
6. Update the credentials path in your configuration

### API Key Acquisition

- **Deepgram**: [Sign up](https://deepgram.com/) for speech-to-text services
- **Tavily**: [Register](https://tavily.com/) for web search API access
- **Groq**: [Get API key](https://groq.com/) for Llama3 model access
- **Google Gemini**: Available through Google AI Studio

## Usage

### Starting the Assistant

```bash
python main.py
```

### Voice Commands Examples

**Calendar Management**
- "Schedule a team meeting for tomorrow at 3 PM"
- "Book a doctor's appointment for Friday at 10 AM"

**Contact Management**
- "Add Sarah Johnson to my contacts, phone number 555-0123"
- "What's Mike's email address?"

**Email Communication**
- "Send an email to Jennifer about the quarterly report"
- "Compose a message to the development team"

**Information Retrieval**
- "Search for the latest news on renewable energy"
- "Find my notes about the marketing strategy"

**Session Management**
- Say "goodbye" to end the conversation

## Project Structure

```
AI-Voice-Assitant/
├── main.py                 # Application entry point
├── requirements.txt        # Python dependencies
├── .env                   # Environment variables (create this)
├── files/                 # Personal knowledge base documents
├── tools/                 # Tool implementations
└── README.md              # Project documentation
```

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow PEP 8 style guidelines
- Add unit tests for new features
- Update documentation for API changes
- Ensure all tests pass before submitting

## Troubleshooting

### Common Issues

**Authentication Errors**
- Verify all API keys are correctly set in `.env`
- Check Google Cloud credentials and permissions

**Speech Recognition Issues**
- Ensure microphone permissions are granted
- Verify Deepgram API key is valid

**Tool Integration Problems**
- Confirm Google APIs are enabled in Cloud Console
- Check service account permissions

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For questions, issues, or suggestions:

- **Email**: aymenMir1001@gmail.com
- **Issues**: [GitHub Issues](https://github.com/danieladdisonorg/AI-Voice-Assitant/issues)
- **Discussions**: [GitHub Discussions](https://github.com/danieladdisonorg/AI-Voice-Assitant/discussions)

## Acknowledgments

- [Deepgram](https://deepgram.com/) for speech processing capabilities
- [Google Cloud](https://cloud.google.com/) for productivity service integrations
- [Tavily](https://tavily.com/) for web search functionality
- [Groq](https://groq.com/) for language model inference

---

**Built with ❤️ for seamless AI-human interaction**
