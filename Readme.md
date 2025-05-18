To structure a function-calling AI agent using open-source tools like LangChain, you’ll follow a modular and extensible architecture. Below is a recommended folder and code structure, which mirrors how Azure Agents work, but with open-source and local tools.

ai-agent/
│
├── agents/
│   └── sales_agent.py          # Defines the agent, LLM, tools, and instructions
│
├── tools/
│   ├── sales_tools.py          # Tools (functions) for sales data
│   └── utility_tools.py        # Additional utilities like file parsing or charts
│
├── data/
│   └── contoso_sales.db        # Example SQLite DB or CSV files
│
├── prompts/
│   └── instructions.txt        # Prompt template with placeholders
│
├── main.py                     # Entrypoint that runs the interaction loop
│
├── requirements.txt
└── .env                        # Optional for secrets and config