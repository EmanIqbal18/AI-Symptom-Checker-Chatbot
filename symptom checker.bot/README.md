# AI Symptom Checker Chatbot

A Python AI powered symptom checker that analyze symptoms from natural language input and provide possible diagnoses with health recommendations.

## Features

- Free text symptom input describe how you feel naturally
- AI does all the medical reasoning (no rule-based logic)
- Returns possible conditions, severity, and actionable recommendations
- Flask based REST API with a chat interface
- Session based conversation history

## Project Link
GitHub Repository:https://github.com/EmanIqbal18/AI-Symptom-Checker-Chatbot

## Setup

```bash
# 1. Clone and enter the project
git clone <repo-url>
cd symptom-checker

# 2. Install dependencies
pip install -r requirements.txt

# 3. Set your Anthropic API key
export ANTHROPIC_API_KEY=your_key_here

# 4. Run
python app.py
# → http://localhost:5000
```


## Project Structure

```
symptom-checker/
├── app.py   
├── history.json
├── dataset.csv    
├── requirements.txt    
├── templates/
│   └── index.html   
|   └── login.html
└── static/
    ├── css/style.css
```


## API

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET`  | `/` | Chat UI |
| `POST` | `/api/chat` | Analyze symptoms `{"message": "..."}` |
| `POST` | `/api/reset` | Reset session |


## Requirements

- Python 3.8+
- Flask
- `anthropic` Python SDK
- Anthropic API key


This project is informational purposes only. Not a substitute for professional medical advice.
