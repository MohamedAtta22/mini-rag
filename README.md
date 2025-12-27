# mini-rag

This is a minimal implementation of the RAG model for question answering.

## Requirements

- python 3.8 or later

### Install Python using MiniConda

1) Download and install MiniConda from [here](https://www.anaconda.com/docs/getting-started/miniconda/main)
2) Create a new environment using the following command: 
```bash
$ conda create -n mini-rag python=3.8
```
3) Active the environment:
```bash
$ conda activate mini-rag
```

### Install UV
1) Follow the CLI installation [here](https://docs.astral.sh/uv/#highlights)

## Installation

### Install the required packages

```bash
$ pip install -r requirements.txt
```

### Setup the environmnet variables

```bash
$ cp .env.example .env
```
set your environment variables in the `.env` file. like the `OPENAI_API_KEY` value.

