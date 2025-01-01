# Agentic AI Repository

Agentic AI is a cutting-edge framework for developing and deploying multiple specialized AI agents. These agents are designed to perform tasks such as web search, financial analysis, and more. The project utilizes advanced AI models and tools to provide robust, efficient, and insightful solutions.

---

## Features

1. **Web Search Agent**
   - Uses DuckDuckGo for retrieving web information.
   - Always includes sources in the response.
   - Leverages the Groq model for enhanced tool usage.

2. **Finance AI Agent**
   - Retrieves financial data such as stock prices, analyst recommendations, and company news using YFinance tools.
   - Presents data in tabular format for better readability.
   - Powered by the Groq model for precise financial insights.

3. **Multi-AI Agent**
   - Combines the capabilities of Web Search Agent and Finance AI Agent.
   - Unified response format adhering to instructions like including sources and using tables.

4. **Playground App**
   - Interactive UI for testing and deploying agents.
   - Built using the `phi` library's Playground module.

---

## Repository Structure

```
Agentic AI/
├── agents/                        # AI agents implementation
│   ├── web_search_agent.py        # Web Search Agent code
│   ├── finance_agent.py           # Finance AI Agent code
│
├── app.py                         # Playground app for interacting with agents
├── requirements.txt               # Python dependencies
├── README.md                      # Project documentation
├── .env                           # Environment variables
└── .gitignore                     # Files to ignore in Git
```

---

## Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/AgenticAI.git
   cd AgenticAI
   ```

2. **Install Dependencies**
   Ensure Python 3.8+ is installed.
   ```bash
   pip install -r requirements.txt
   ```

3. **Environment Variables**
   Create a `.env` file in the root directory with the following keys:
   ```env
   OPENAI_API_KEY=your_openai_api_key
   PHI_API_KEY=your_phi_api_key
   ```

4. **Run the Playground App**
   ```bash
   python app.py
   ```
   The app will be available at `http://localhost:8000`.

---

## Usage Examples

### Web Search Agent
```python
response = web_search_agent.print_response("Find the latest news about AI technologies.", stream=True)
print(response)
```

### Finance AI Agent
```python
response = finance_agent.print_response("Provide analyst recommendations and company news for Tesla.")
print(response)
```

### Multi-AI Agent
```python
response = multi_ai_agent.print_response("Summarize analyst recommendation and share the latest news for NVDA.", stream=True)
print(response)
```

---

## Contributing

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add some feature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Acknowledgments

Special thanks to the developers of the `phi` library, OpenAI, and YFinance for their incredible tools and support.


