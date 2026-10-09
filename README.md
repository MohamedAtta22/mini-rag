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

### Install Python using UV

1) Follow the CLI installation [here](https://docs.astral.sh/uv/#highlights)
2) Install Python 3.12 (UV downloads a standalone build if needed):
```bash
$ uv python install 3.8.20
```

## Installation

### Install the required packages

This project uses `pyproject.toml` as the single source of truth
(mirrored in `src/requirements.txt` for pip users).

```bash
$ uv sync
```

Pip fallback:

```bash
$ pip install -r src/requirements.txt
```

### Setup the environmnet variables

```bash
$ cp src/.env.example src/.env
```
set your environment variables in the `src/.env` file. like the `OPENAI_API_KEY` value.

## Run Docker Compose Services
```bash
$ cd docker
$ cp .env.example .env
```
- update `.env` with your credentials

```bash
$ cd docker
$ sudo docker compose up -d
```

## Run the FastAPI server

```bash
$ cd src
$ uvicorn main:app --reload --host 0.0.0.0 --port 5000
```
