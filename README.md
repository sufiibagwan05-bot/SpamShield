# 🛡️ Email Spam Detection System

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)
![Accuracy](https://img.shields.io/badge/Accuracy-97.8%25-brightgreen.svg)

ML-powered email spam detection with interactive web interface

## 🌐 Live Demo

**Try it now:** [https://spamshield-project.streamlit.app/](https://spamshield-project.streamlit.app/)

No installation required - test the system directly in your browser!

## 🚀 Quick Start

```bash
git clone https://github.com/Sahas2711/spam-email-detection.git
cd spam-email-detection
pip install -r requirements.txt
streamlit run app.py
```

Open http://localhost:8501

## ✨ Features

- **Real-time Detection** - Instant spam classification
- **Batch Processing** - Analyze multiple emails via CSV
- **Interactive Dashboard** - Visual analytics with charts
- **97.8% Accuracy** - Multinomial Naive Bayes + TF-IDF
- **Privacy-First** - Local processing, no data storage

## 📦 Installation

### Local Setup
```bash
pip install -r requirements.txt
streamlit run app.py
```

### Docker
```bash
docker build -t spam-detector .
docker run -p 8501:8501 spam-detector
```

## 🚀 Deployment

### Streamlit Cloud
1. Fork repository
2. Connect to [Streamlit Cloud](https://streamlit.io/cloud)
3. Deploy from GitHub


## 📊 Performance

| Metric | Score |
|--------|-------|
| Accuracy | 97.8% |
| Precision | 100.0% |
| Recall | 83.9% |
| F1-Score | 91.2% |

## 📄 Sample Data

For batch testing, use this sample CSV format:

**Download:** [sample_emails.csv](sample_emails.csv)

```csv
message,actual_label
"Congratulations! You've won $1,000,000!",spam
"Hi John, hope you're doing well.",ham
"URGENT: Your account will be closed!",spam
"Meeting scheduled for tomorrow at 3 PM",ham
```

## 💻 Usage

### Web Interface
1. Train model using sidebar
2. Analyze emails (manual/batch/examples)
3. View results with confidence scores

### API
```python
from model_trainer import SpamDetector

detector = SpamDetector()
detector.train_model()
result = detector.predict("Your email text")
print(f"Prediction: {result['label']}")
```

## 📁 Files

```
spam-email-detection/
├── app.py              # Streamlit app
├── model_trainer.py    # ML model
├── requirements.txt    # Dependencies
├── Dockerfile         # Docker setup
└── README.md          # This file
```

## 🔧 Tech Stack

- **ML**: Scikit-learn, Pandas, NumPy
- **Web**: Streamlit, Plotly
- **Deploy**: Docker, Heroku, Streamlit Cloud

## 📝 License

MIT License

## 👤 Author

**Sahas Nagar**
- GitHub: [Sahas2711](https://github.com/Sahas2711)
- Email: sahasnagar1234@gmail.com

---

⭐ Star this repo if helpful!