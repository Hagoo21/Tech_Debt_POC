# Tech Debt POC

This project implements a multi-agent system using the OpenAI Agents SDK, allowing multiple AI agents to work together to accomplish complex tasks.

## Prerequisites

- Python 3.12 or higher
- An OpenAI API key
- A Tavily API key (for search capabilities)
- uv (Python package installer and resolver)

## Installation

1. Clone the repository:
```bash
git clone <your-repository-url>
cd Tech_Debt_POC
```

2. Install uv if you haven't already:
```bash
pip install uv
```

3. Install dependencies using uv:
```bash
uv pip install -e .
```

## Environment Setup

Create a `.env` file in the root directory with the following variables:
```
OPENAI_API_KEY=your_openai_api_key_here
TAVILY_API_KEY=your_tavily_api_key_here
```

## Project Structure

```
tech_debt_poc/
├── agents_and_tools/
│   ├── agent_tools/     # Custom tools for agents
│   ├── data/           # Data files
│   ├── miscs/          # Miscellaneous utilities
│   ├── models/         # Agent model definitions
│   ├── prompts/        # Agent prompts
│   ├── schemas/        # Data schemas
│   └── multi_agents.py # Main multi-agent implementation
├── pyproject.toml      # Project dependencies
└── README.md          # This file
```


## Dependencies

The project uses the following main dependencies:
- openai-agents >= 0.0.3
- pydantic >= 2.10.6
- tavily-python >= 0.5.1
- python-dotenv >= 0.9.9
