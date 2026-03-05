# AI Travel Planner with Multi-Agent A2A Protocol

An AI-powered travel planner built using agent-to-agent (A2A) collaboration. Specialized agents for flights, hotels, weather, and attractions work together under a root agent to handle complex travel planning queries through a CLI interface.

## Tech Stack

- Python
- Google Gemini (via Agent Development Kit)
- OpenWeatherMap API
- A2A (Agent2Agent) Protocol

## Project Structure

- `agents/` — Individual specialized agents (flights, hotels, weather, attractions)
- `root_agent/` — Root agent that coordinates and delegates to sub-agents
- `cli/` — Command-line interface connecting the user to the root agent

## Setup

1. Clone the repo
```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
```

2. Install dependencies
```bash
   pip install -r requirements.txt
```

3. Add your API keys in a `.env` file
```
   GEMINI_API_KEY=your_key_here
   OPENWEATHERMAP_API_KEY=your_key_here
```

4. Run the planner
```bash
   python main.py
```

## Agents Overview

| Agent | Role |
|---|---|
| Attractions Agent | Suggests places to visit |
| Flight Agent | Finds flight options |
| Hotel Agent | Recommends accommodations |
| Weather Agent | Fetches live weather via OpenWeatherMap |
| Root Agent | Delegates tasks and coordinates all agents |

## Learning Outcomes

- Build specialized AI agents using Google ADK
- Implement A2A multi-agent collaboration
- Connect agents to a root coordinator
- Run an async multi-agent system via CLI