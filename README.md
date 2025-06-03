# Samantha - Code Teaching Assistant

**Samantha** is a local AI-powered code teaching assistant built using [Gradio](https://gradio.app/) and a local [Ollama](https://ollama.com/) model server. It uses a conversational history to provide better and more context-aware code-related answers.

## Features

* Interacts with a local LLM model served via Ollama
* Maintains chat history for context-aware responses
* Provides a simple web interface using Gradio
* Designed to help users with coding questions
* you can also save ouput by clicking flag option,that saves in your local folder

## Requirements

Install dependencies with:

```cmd
pip install -r requirements.txt
```

Make sure you have [Ollama](https://ollama.com/) installed and running locally.

## Files

* `app.py`: Main Python file to run the Gradio interface
* `Modelfile`: Defines the local model behavior and prompt system
* `requirements.txt`: Required Python packages

## Usage

1. **Start your local model server** using Ollama:

   ```cmd
   ollama create Samantha -f Modelfile
   ```

2. **Run the application**:

   ```cmd
   python app.py
   ```

3. **Open your browser** — Gradio will launch a web interface where you can enter code-related questions.

## Notes

* Make sure the Ollama server is running at `http://localhost:11434`
* The assistant name is **Samantha**, created by **Brahme**
* Modify the `Modelfile` to adjust system prompts or model parameters