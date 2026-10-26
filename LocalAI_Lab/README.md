# FSTT Local AI Assistant

Flask web UI -> Ollama -> local LLM, with a TF-IDF retriever over `documents/`, conversation history, structured (JSON) answers and response-time display.

## Setup
```bash
ollama pull qwen3.5
pip install flask requests psutil pandas
```

## Run
```bash
cd source
python app.py
python chatbot.py
python benchmark.py qwen3.5 gemma3
```
Open http://127.0.0.1:5001 for the web interface. Environment variables: `MODEL`, `OLLAMA_URL`, `PORT`.
