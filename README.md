# DeepResearchAgent

A multi-agent system for conducting **deep research** on any topic, generating comprehensive reports, and delivering them via email. It combines automated planning, web search, synthesis, report writing, and email delivery into one seamless pipeline.

## 🚀 Features

- **Intelligent Planning**: Automatically generates multiple strategic search queries based on your research topic
- **Web Search & Analysis**: Executes web searches and summarizes results concisely
- **Comprehensive Reporting**: Synthesizes findings into detailed, structured Markdown reports (5-10 pages)
- **Email Integration**: Sends reports as formatted HTML emails
- **Process Transparency**: Shows execution traces for debugging and transparency
- **Simple Interface**: Clean Gradio UI for easy interaction

## ⚙️ Tech Stack

- **Python 3.10+**
- **[Gradio](https://gradio.app/)** - User interface
- **[Pydantic](https://docs.pydantic.dev/)** - Data validation
- **[SendGrid](https://sendgrid.com/)** - Email delivery
- **[python-dotenv](https://pypi.org/project/python-dotenv/)** - Environment management
- **AsyncIO** - Async orchestration
- **Custom Multi-Agent Framework** - Built with GPT-4o-mini & tracing

## 📂 Project Structure

```
deep-research-agent/
├── app.py                 # Gradio UI entry point
├── research_manager.py    # Multi-agent workflow orchestrator
├── planner_agent.py       # Search query planning agent
├── search_agent.py        # Web search & summarization agent
├── writer_agent.py        # Report writing agent
├── email_agent.py         # Email delivery agent
├── agents/                # Multi-agent framework components
│   ├── runner.py
│   ├── agent.py
│   ├── tools.py
│   └── tracing.py
├── requirements.txt       # Python dependencies
└── README.md             # This file
```

## 🚀 Getting Started

### Prerequisites

- Python 3.10 or higher
- OpenAI API key
- SendGrid API key

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/deep-research-agent.git
cd deep-research-agent
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

### Configuration

Create a `.env` file in the root directory:

```env
SENDGRID_API_KEY=your_sendgrid_api_key
OPENAI_API_KEY=your_openai_api_key
```

### Running the Application

```bash
python app.py
```

The Gradio interface will open in your browser automatically.

## 💻 Usage

1. **Enter your research topic** in the text input field
   - Example: "Impact of AI on cybersecurity"
   - Example: "How will quantum computing disrupt the finance sector?"

2. **Click "Run"** to start the research process

3. **Monitor progress** via the trace link displayed in the console

4. **Receive results** - The final report will be displayed in the interface and sent to your configured email

## 📋 Example Workflow

**Input:**
```
How will quantum computing disrupt the finance sector?
```

**Process:**
1. 🧠 Plans 5 strategic web searches
2. 🔍 Executes searches and summarizes findings
3. 📄 Builds a comprehensive 5-10 page Markdown report
4. 📧 Emails the formatted report to your inbox

**Output:**
- Detailed analysis of quantum computing applications in finance
- Risk assessments and timeline predictions
- Key players and investment opportunities
- Regulatory considerations and challenges

## 🔧 Configuration Options

You can customize the behavior by modifying:
- Number of search queries generated
- Report length and structure
- Email formatting and recipients
- Search result processing depth

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

Please open an issue first to discuss major changes.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🌟 Acknowledgments

- Inspired by autonomous multi-agent research workflows
- Powered by OpenAI GPT-4o-mini and Gradio
- Built with modern Python async patterns

---
