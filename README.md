# ghost.py
👻 A spooky AI ghost storyteller powered by Ollama and the open-weight Gemma 3 1B model. Generate eerie stories directly in your terminal with local AI, enhanced privacy, and offline support after downloading the model.

# 👻 Ghost in the Terminal

A spooky AI ghost storyteller powered by a locally running open-weight language model.

Ask the ghost questions and receive eerie stories about abandoned servers, forgotten programmers, and mysterious machines.

## Features

- Runs locally using Ollama and Gemma 3 1B.
- No cloud AI API key required.
- Works offline after the model has been downloaded.
- Simple interactive Python terminal interface.
- Uses Python's standard library for API requests.

## Requirements

- Python 3.9 or newer
- [Ollama](https://ollama.com/download)
- Enough memory to run the selected model

## Installation

### 1. Install Ollama

Download Ollama from https://ollama.com/download.

### 2. Download the model

Open PowerShell or a terminal and run:

```bash
ollama pull gemma3:1b
```

### 3. Download this repository

Clone it with Git:

```bash
git clone https://github.com/YOUR-USERNAME/ghost-in-the-terminal.git
cd ghost-in-the-terminal
```

Alternatively, download the repository as a ZIP from GitHub and extract it.

Replace `YOUR-USERNAME` with your GitHub username.

### 4. Run the ghost

```bash
python ghost.py
```

On some Windows installations, use:

```powershell
py ghost.py
```

Ask a spooky question when prompted. Type `quit` to exit.

## How It Works

Python sends prompts to Ollama's local HTTP API at `localhost:11434`. Ollama runs Gemma 3 1B and returns the generated story.

## Why Open AI?

Using a locally running open-weight model gives users more control over their data and experimentation. After the initial model download, the application can work without internet access, as long as the model is installed and Ollama is running.

## Theme

Built for Hacktoberfest Open-Source AI Challenge — Week 4: Ghost in the Machine.

Challenge: https://dev.to/challenges/hacktoberfest-week4-2026-10-26

## License

MIT
