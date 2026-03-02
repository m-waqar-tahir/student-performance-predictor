# 🎓 Student Performance Predictor

> A Machine Learning project to predict student pass/fail outcomes using behavioral and academic features.

**By Muhammad Waqar Tahir** — BS Computer Science, GCU Faisalabad

---

## 📌 Problem Statement

Early identification of at-risk students allows educators to intervene before it's too late. This project builds a binary classification model that predicts whether a student will **pass or fail** based on easily measurable behavioral data — making it a practical **AI for Social Good** application.

---

## 🔍 Features Used

| Feature | Description |
|---|---|
| `study_hours` | Weekly study hours |
| `attendance_pct` | Attendance percentage (30–100%) |
| `previous_scores` | Score in previous exams (out of 100) |
| `sleep_hours` | Average nightly sleep |
| `extracurricular` | Participation in activities (Yes/No) |

**Target:** `passed` — 1 = Pass, 0 = Fail

> **Note:** This project uses a synthetic dataset generated to mirror the statistical properties of real student performance data. It is designed to work fully offline without requiring any external data download.

---

## 🧠 ML Pipeline

1. **Data Generation & Loading** — 1,000 student records with realistic distributions
2. **EDA** — Distribution plots, correlation heatmap, pass rate analysis
3. **Preprocessing** — 80/20 train-test split with stratification
4. **Model 1: Logistic Regression** — Interpretable baseline model
5. **Model 2: Random Forest** — Ensemble model with improved accuracy
6. **Evaluation** — Accuracy, confusion matrix, classification report
7. **Feature Importance** — Identifies top predictors using RF importance scores
8. **Live Prediction** — Demo: input any student's stats and get a pass/fail prediction

---

## 📊 Results

| Model | Accuracy |
|---|---|
| Logistic Regression | ~78% |
| Random Forest | **80%+** |

The Random Forest model outperformed Logistic Regression and identified **previous exam scores** and **study hours** as the strongest predictors of student success.

---

## 🖼️ Visualizations

The notebook generates and saves the following charts:
- `eda_distributions.png` — Feature distributions by pass/fail
- `correlation_heatmap.png` — Feature correlation matrix
- `model_comparison.png` — Confusion matrices + accuracy comparison
- `feature_importance.png` — Top predictors bar chart

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install -r requirements.txt
```

### Run

Open the notebook in Jupyter or Google Colab:

```bash
jupyter notebook student_performance_predictor.ipynb
```

Run all cells top to bottom (Kernel → Restart & Run All).

---

## 📦 Requirements

See `requirements.txt` for the full list. Main dependencies:

- Python 3.8+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

---

## 💡 Future Improvements

- Collect and use real student data from Pakistani schools
- Add socioeconomic and internet access features
- Test XGBoost and neural network models
- Build a simple web interface using Streamlit

---

## 👤 Author

**Muhammad Waqar Tahir**
📧 waqartahir480@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/waqar-tahir-445a072b9)
🔗 [GitHub](https://github.com/m-waqar-tahir)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
