# StockPicker Crew

Welcome to the StockPicker Crew project, powered by [crewAI](https://crewai.com). This is a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. The goal is to enable agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities.

## Installation

Python requirements: Python >=3.10 <3.14. 
This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First,install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

(Optional) Lock the dependencies and install them by using the CLI command:
```bash
crewai install
```
### Customizing

**Add `OPENAI_API_KEY` into the `.env` file**

- Modify `src/stock_picker/config/agents.yaml` to define agents
- Modify `src/stock_picker/config/tasks.yaml` to define tasks
- Modify `src/stock_picker/crew.py` to add own logic, tools and specific args
- Modify `src/stock_picker/main.py` to add custom inputs for  agents and tasks

## Running the Project

To kickstart the crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the stock_picker Crew, assembling the agents and assigning them tasks as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding The Crew

The stock_picker Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in crew.

