# 📚 Virtual Research Assistant

A powerful research assistant that helps users explore academic papers by fetching, summarizing, and analyzing research content using AI.

## 🌟 Features

- **Paper Search**: Fetches relevant research papers from ArXiv based on user queries
- **AI-Powered Summarization**: Generates concise summaries of research papers
- **Advantages/Disadvantages Analysis**: Provides detailed pros and cons analysis for each paper
- **Interactive UI**: Built with Streamlit for a seamless user experience
- **Expandable Search**: Automatically expands search to related topics when fewer papers are found

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **AI/ML**: 
  - Groq LLM (llama-3.3-70b-versatile model)
  - AutoGen for AI agent orchestration
- **APIs**: 
  - ArXiv API for research paper fetching
- **Python Libraries**:
  - `requests`: For API calls
  - `xml.etree.ElementTree`: For XML parsing
  - `python-dotenv`: For environment variable management
  - `autogen`: For AI agent implementation

## 📋 Prerequisites

- Python 3.x
- Groq API key

## 🚀 Getting Started

1. **Clone the repository**

```bash
git clone <repository-url>
cd virtual-research-assistant
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Set up environment variables**

Create a `.env` file in the root directory:

```env
GROQ_API_KEY=your_groq_api_key_here
```

4. **Run the application**

```bash
streamlit run app.py
```

## 🏗️ Project Structure

```
├── app.py                 # Main Streamlit application
├── agents.py             # AI agents implementation
├── data_loader.py        # Data fetching and processing
├── .env                  # Environment variables
└── README.md            # Project documentation
```

## 💻 Usage

1. Launch the application
2. Enter a research topic in the search field
3. Click "Search" to fetch and analyze papers
4. View summaries and analyses for each paper
5. Click paper links to access original sources

## 🤖 AI Agents

### Summarizer Agent
- Generates concise summaries of research papers
- Focuses on key findings and contributions

### Advantages/Disadvantages Agent
- Analyzes papers for strengths and weaknesses
- Provides structured pros and cons analysis

## 📊 Data Sources

### ArXiv
- Fetches up to 5 relevant papers
- Expands search using related topics when needed
- Provides paper titles, summaries, and links

## ⚙️ Configuration

The application uses the following configurations:

- **LLM Config**:
  - Model: llama-3.3-70b-versatile
  - API Provider: Groq
  - Human Input Mode: NEVER
  - Code Execution: Disabled

## 🔒 Security

- API keys are stored securely in environment variables
- No sensitive data is stored or logged

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- ArXiv for providing access to research papers
- Groq for AI model access
- AutoGen for AI agent framework
- Streamlit for the UI framework
