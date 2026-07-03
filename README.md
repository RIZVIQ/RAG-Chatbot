# RAG - QA

A Retrieval Augmented Generation (RAG) app for ingesting your own data and chatting with it through a clean, interactive UI.

## Requirements

This project relies on `uv` as the package manager. Any other package manager works fine too — swap in whichever you prefer.

### Setting up uv

`curl -LsSf https://astral.sh/uv/install.sh | sh`

### Checking the version

`uv --version`

## Getting the Project

Grab the code by cloning it or downloading the ZIP:

`git clone https://github.com/RIZVIQ/RAG-Chatbot`

## Preparing Your Environment

### Spin up a virtual environment

`uv venv`

#### Turn it on

`source .venv/bin/activate`

#### Pull in the dependencies

`uv sync`

## Using the App

### Step 1: Load your data

Run the ingestion script to process and store your data:
`uv run ingest.py`

### Step 2: Fire it up

Drop your Groq API key into the `.env` file, then get the Streamlit app running:
`uv run streamlit run app.py`

## A Few Things to Keep in Mind

- Your data files need to be ready beforehand, and `config.py` should be updated to match your setup.
- The app opens automatically in your browser once Streamlit is running.
- Run `deactivate` anytime you want to exit the virtual environment.