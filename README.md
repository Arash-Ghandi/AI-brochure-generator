# AI-brochure-generator (Ollama & Gradio)

An intelligent and automated tool to convert company website content into professional business and promotional brochures using Large Language Models (LLMs).

## Key Features
- Secure Environment Management: Utilizing .env files to prevent API key exposure.
- Unified Client Architecture: Demonstrating how a single client interface (OpenAI Client) can communicate with different AI backends.
- Local LLM Support: Running and testing prompts completely offline on your own machine using Ollama.

## Prerequisites
To run this notebook, you will need:
- Python 3.11.3
- Ollama installed and running (for the local model section)
- **Smart Web Scraping:** Automatically crawls the website and gathers textual information.
- **AI-Powered Filtering:** Selects the most relevant pages (e.g., About Us, Products, Investors) using an LLM.
- **Structured Content Generation:** Creates well-structured and standard business brochures.
- **Easy User Interface:** Features a simple web-based UI powered by Gradio.

## Getting Started
- Clone the repository.
- Create a .env file in the root directory of the project and configure the following environment variables:

```bash
OLLAMA_BASE_URL=http://localhost:11434/v1
OLLAMA_MODEL=llama3
```
## Setup
- Using Python + venv

bash:
```BASH
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```
Install Dependensies

- Using UV (recommended)

After selecting the Python version, create a virtual environment with uv:

````
uv venv
````
Then install the dependencies:

````
uv pip install -r requirements.txt --refresh
````