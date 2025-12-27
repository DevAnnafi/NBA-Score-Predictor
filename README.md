# 🏀 NBA Score Predictor

An end-to-end machine learning application that predicts **NBA game scores and win probabilities** using historical data, feature engineering, and regression models. The system is designed as a production-style ML pipeline, exposed via a REST API and built with extensibility in mind.

---

## 🚀 Overview

The NBA Score Predictor ingests historical NBA game data, engineers team- and game-level features (pace, offensive/defensive ratings, rest days, home-court advantage), and trains machine learning models to predict final scores and win probabilities for upcoming matchups.

This project emphasizes:
- Applied machine learning
- Feature engineering discipline
- Proper model evaluation and backtesting
- Clean backend architecture
- Portfolio-ready system design

---

## 🔮 Features

- 🏀 Predict final scores for upcoming NBA games  
- 📊 Win probability estimation  
- 🔁 Rolling averages (last N games)  
- 🏠 Home vs away performance modeling  
- ⏱ Rest-day and schedule effects  
- 📡 REST API for real-time predictions  
- 📈 Evaluation with MAE, RMSE, and accuracy metrics  

---

## 🧠 Modeling Approach

### Regression (Score Prediction)
- Linear Regression (baseline)
- Random Forest / Gradient Boosting (planned)

### Classification (Win Probability)
- Logistic Regression on score differential
- Probabilistic calibration

Scores are predicted **separately** for home and away teams to improve accuracy.

---

## 🏗 System Architecture

```
Data Source
↓
Data Ingestion
↓
Feature Engineering
↓
Model Training
↓
Evaluation & Backtesting
↓
REST API (FastAPI)
↓
Client / Frontend
```

---

## 🛠 Tech Stack

**Backend & ML**
- Python
- Pandas / NumPy
- scikit-learn
- FastAPI

**Data**
- Historical NBA game data (CSV / API-based)
- SQLite / PostgreSQL (planned)

**Deployment**
- Render / Railway (planned)
- Vercel (frontend)

---

## 📁 Project Structure

```
nba-score-predictor/
│── data/ # Raw and processed datasets
│── notebooks/ # EDA and experimentation
│── src/
│ ├── ingestion/ # Data loading
│ ├── features/ # Feature engineering
│ ├── models/ # Training & evaluation
│ ├── api/ # FastAPI endpoints
│── tests/ # Unit tests
│── README.md

```


---

## 📊 Evaluation Metrics

- **MAE** (Mean Absolute Error)
- **RMSE** (Root Mean Squared Error)
- **Accuracy & Log Loss** (win probability)
- Rolling-window backtesting by season

---

## ⚠️ Disclaimer

This project is for **educational and analytical purposes only**.  
It is **not** intended for gambling or financial decision-making.

---

## 📌 Roadmap

- [ ] Injury-adjusted predictions  
- [ ] Live in-game win probability  
- [ ] SHAP-based model explainability  
- [ ] React frontend dashboard  
- [ ] Automated retraining pipeline  

---

## 👤 Author

**Annafi Islam**  
Computer Science Graduate | Cybersecurity & Applied ML  
GitHub: https://github.com/DevAnnafi

---

## ⭐ Why This Project Matters

This repository demonstrates real-world skills in:
- Machine learning pipelines
- Feature engineering
- Model evaluation discipline
- API design
- Production-oriented thinking

Ideal for **software engineering**, **data**, and **ML-focused** roles.
