# DeepResearchAgent

A multi-agent system for conducting **deep research** on any topic, generating a comprehensive report, and sending it via email.  
It combines automated planning, web search, synthesis, report writing, and email delivery into one seamless pipeline.

## 🚀 Features

✅ Automatically plans multiple search queries based on your topic  
✅ Executes web searches & summarizes results concisely  
✅ Synthesizes findings into a detailed, structured Markdown report (5-10 pages)  
✅ Sends the report as a formatted HTML email  
✅ Shows process traces for transparency & debugging  
✅ Simple Gradio UI for user input

---

## ⚙️ Tech Stack

- **Python 3.10+**
- [Gradio](https://gradio.app/) - for UI
- [Pydantic](https://docs.pydantic.dev/) - data validation
- [SendGrid](https://sendgrid.com/) - sending emails
- [dotenv](https://pypi.org/project/python-dotenv/) - environment management
- Async orchestration with `asyncio`
- Custom multi-agent framework with GPT-4o-mini & tracing

---

## 📂 Project Structure

deep-research-agent/
├── app.py # Gradio UI to start the research process
├── research_manager.py # Orchestrates the multi-agent workflow
├── planner_agent.py # Plans search queries
├── search_agent.py # Performs web searches & summaries
├── writer_agent.py # Writes a comprehensive Markdown report
├── email_agent.py # Sends the final report via email
├── agents/ # Your multi-agent framework (Runner, Agent, tools, tracing, etc.)
└── requirements.txt # Python dependencies

yaml
Copy
Edit

---

## 🚀 Getting Started

### 🔧 Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/yourusername/deep-research-agent.git
cd deep-research-agent
pip install -r requirements.txt
🔑 Environment Variables
Create a .env file in the root directory:

ini
Copy
Edit
SENDGRID_API_KEY=your_sendgrid_api_key
OPENAI_API_KEY=your_openai_api_key
▶️ Run the App
bash
Copy
Edit
python app.py
It will open a Gradio interface in your browser.

💻 Usage
Enter a topic or research question in the textbox (e.g. Impact of AI on cybersecurity).

Click Run.

Watch the trace link in the console for step-by-step execution.

The final report will be displayed and sent to your configured email.

📝 Example Flow
Input:

nginx
Copy
Edit
How will quantum computing disrupt the finance sector?
Output:

Plans 5 strategic web searches

Summarizes key findings

Builds a 5-10 page Markdown report

Emails the formatted report to your inbox

🤝 Contributing
PRs welcome! Open an issue first to discuss changes.

🌟 Acknowledgments
Inspired by autonomous multi-agent research workflows

Powered by OpenAI GPT-4o-mini and Gradio
