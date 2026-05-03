# AI Symptom Checker Chatbot

A Python AI powered symptom checker that analyze symptoms from natural language input and provide possible diagnoses with health recommendations.


## Features

- AI powered disease prediction from symptoms
- Confidence scores & severity classification (Mild / Moderate / Severe)
- Health recommendations per disease
- Emergency alert for life threatening symptom combinations
- Per user diagnosis history
- Dark futuristic UI with autocomplete symptom input

## Project Link
GitHub Repository: https://github.com/EmanIqbal18/AI-Symptom-Checker-Chatbot

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python, Flask |
| AI / NLP | Groq API — LLaMA 3.3 70B | AI logic
| Frontend | HTML, CSS, JavaScript |
| Data | CSV dataset (41 diseases) |
| Storage | JSON file |

---

## Project Structure

```
symptom bot/
├── app.py              
├── dataset.csv         
├── history.json         
├── requirements.txt    
├── .env                
├── templates/
│   ├── login.html      
│   └── index.html      
└── static/
    └── style.css       
```

---

## 🚀 Setup & Run

**1. Install dependencies**
```bash
pip install -r requirements.txt
```

**2. Add your Groq API key**

Get a free key at [console.groq.com](https://console.groq.com), then add it to `.env`:
```
GROQ_API_KEY=gsk_your_key_here
```

**2. Run the app**
```bash
python app.py
```

Visit `http://localhost:5000` in your browser.



## How It Works

1. User logs in and enters symptoms (e.g. `fever, cough, headache`)
2. Flask sends the symptoms to the Groq LLaMA 3.3 model
3. The AI returns a structured JSON response with predicted diseases
4. Results are displayed with confidence rings, severity badges, and recommendations
5. Each diagnosis is saved to `history.json`


## Disclaimer

SymptoBot is an academic project for educational purposes only. It is **not a substitute** for professional medical advice, diagnosis, or treatment. Always consult a qualified doctor.


## License

MIT License free to use for educational purposes.

---
