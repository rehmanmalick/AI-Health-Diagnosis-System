# 🏥 AI-Driven HealthBot & Disease Diagnosis System

A Flask-based web application that uses Machine Learning to predict the risk of multiple diseases and includes an AI-powered Health Chatbot (Dia).

---

## 🚀 Features

- 🩸 **Diabetes Prediction**
- ❤️ **Heart Disease Prediction**
- 🫘 **Kidney Disease Prediction**
- 🫀 **Liver Disease Prediction**
- 🎗️ **Breast Cancer Prediction**
- 🤖 **AI Health Chatbot (Dia)**
- 🔐 **User Authentication (Login/Signup)**

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, Flask |
| ML Models | Scikit-learn, TensorFlow/Keras |
| Chatbot | NLTK, Keras Neural Network |
| Database | SQLite, Flask-SQLAlchemy |
| Frontend | HTML, CSS, Bootstrap |

---

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.8 or higher
- Git

---

### Step 1 — Clone the Repository

```bash
git clone https://github.com/rehmanmalick/AI-Health-Diagnosis-System.git
cd AI-Health-Diagnosis-System
```

---

### Step 2 — Create Virtual Environment

```bash
python -m venv venv
```

---

### Step 3 — Activate Virtual Environment

**Windows:**
```bash
venv\Scripts\activate
```

**Mac/Linux:**
```bash
source venv/bin/activate
```

---

### Step 4 — Install Dependencies

```bash
pip install -r requirements.txt
```

> ⚠️ This may take 3-5 minutes (TensorFlow is large)

---

### Step 5 — Train Chatbot Model (First Time Only)

```bash
python training.py
```

> This will train the AI chatbot and save `model.h5`, `texts.pkl`, `labels.pkl`
> Takes about 1-2 minutes

---

### Step 6 — Run the Application

```bash
python app.py
```

---

### Step 7 — Open in Browser

```
http://127.0.0.1:5000
```

---

## 📋 Quick Start (All Commands Together)

```bash
git clone https://github.com/rehmanmalick/AI-Health-Diagnosis-System.git
cd AI-Health-Diagnosis-System
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python training.py
python app.py
```

---

## 🗂️ Project Structure

```
AI-Health-Diagnosis-System/
├── app.py                          # Main Flask application
├── training.py                     # Chatbot model training script
├── data.json                       # Chatbot intents and responses
├── diabetes.csv                    # Diabetes dataset
├── requirements.txt                # Python dependencies
├── model.h5                        # Breast cancer model (Keras)
├── model.pkl                       # Breast cancer model (sklearn)
├── model1.pkl                      # Heart disease model
├── kidney_model.pkl                # Kidney disease model
├── liver_model.pkl                 # Liver disease model
├── diabetes-prediction-rfc-model.pkl  # Diabetes model
├── texts.pkl                       # Chatbot vocabulary
├── labels.pkl                      # Chatbot classes
├── Templates/                      # HTML templates
│   ├── index.html
│   ├── login.html
│   ├── signup.html
│   ├── dashboard.html
│   ├── chatbot.html
│   ├── diabetes.html
│   ├── heart.html
│   ├── kidney.html
│   ├── liver.html
│   └── cancer.html
└── Static/                         # CSS and images
```

---

## 💡 How to Use

1. **Signup** — Create a new account
2. **Login** — Login with your credentials
3. **Dashboard** — Select a disease to predict
4. **Fill Form** — Enter patient details
5. **Predict** — Get risk assessment result
6. **Chatbot** — Ask health questions to Dia

---

## ⚠️ Common Issues

**`no such table: user` error:**
```bash
python -c "from app import app, db; app.app_context().__enter__(); db.create_all()"
```

**Model version warning** — Ignore, app works fine

**Slow startup** — Normal, TensorFlow takes time to load

---

## 👨‍💻 Developer

**rem!** — [GitHub](https://github.com/rehmanmalick)
