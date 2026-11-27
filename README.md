# LangGraph Workflows

This repository contains Jupyter notebooks exploring LangGraph workflows, from a basic installation check to examples involving BMI, batsman data, language models, and UPSC essay writing.

## Notebooks

| Notebook | Description |
| --- | --- |
| `0-test-installation.ipynb` | Checks that LangGraph can be imported and used. |
| `1-bmi-workfflow.ipynb` | Demonstrates a BMI workflow using a LangGraph state graph. |
| `2-simple-LLM-workflow.ipynb` | Demonstrates a simple LLM workflow with LangGraph. |
| `4-batsman-workflow.ipynb` | Demonstrates a batsman-related workflow using a LangGraph state graph. |
| `5-upsc-essay-workflow.ipynb` | Demonstrates an essay-writing workflow using LangGraph and an LLM. |

## Requirements

- Python 3.10 or later
- Jupyter Notebook
- API keys for any notebook that calls a hosted language model

## Setup

From the project directory, create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the packages used by the notebooks:

```bash
python -m pip install --upgrade pip
python -m pip install jupyter ipykernel langgraph langchain-google-genai langchain-groq python-dotenv pydantic
```

Start Jupyter:

```bash
jupyter notebook
```

Open a notebook and select the Python kernel for this virtual environment.

## API keys

Some LLM examples need provider API keys. Create a `.env` file in the project directory for the keys used by the notebook, for example:

```dotenv
GROQ_API_KEY=your_groq_api_key
GOOGLE_API_KEY=your_google_api_key
```

Only add the key required by the provider used in a notebook. Keep `.env` private; it is excluded from Git. Never paste real API keys into notebook cells or commit them to the repository.
