# 🍽️ Sentiment Analysis of Google Reviews
### Restaurants in Majitar, East Sikkim (PIN: 737136)

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange?logo=scikit-learn)
![NLP](https://img.shields.io/badge/NLP-Sentiment%20Analysis-green)
![Assignment](https://img.shields.io/badge/B.Tech-NLP%20Assignment-purple)

---

## 📌 Overview

This project performs **Sentiment Analysis** on real Google Reviews from restaurants in **Majitar, East Sikkim, India**.  
Each review is automatically classified as **Positive**, **Negative**, or **Neutral** using classical Machine Learning techniques.

> **B.Tech NLP Assignment** — Natural Language Processing

---

## 📁 Project Structure

```
├── model_fixed.py     # Main Python script (fully commented)
├── dataset.csv        # 20 Google reviews with sentiment labels
├── requirements.txt   # Python dependencies
└── README.md          # This file
```

---

## 🧠 Techniques Used

| Component | Details |
|-----------|---------|
| **Preprocessing** | Lowercasing, removing special characters |
| **Feature Extraction** | TF-IDF (Term Frequency – Inverse Document Frequency) |
| **Model 1** | Multinomial Naive Bayes |
| **Model 2** | Logistic Regression |
| **Evaluation** | Accuracy, Precision, Recall, F1-Score |

---

## 📊 Dataset

- **Location**: Majitar, East Sikkim (PIN: 737136)
- **Total Reviews**: 20
- **Classes**: `positive` · `negative` · `neutral`

| Sentiment | Count | Share |
|-----------|-------|-------|
| Positive  | 13    | 65%   |
| Negative  | 6     | 30%   |
| Neutral   | 1     | 5%    |

> ⚠️ **Class Imbalance**: The dataset is skewed toward positive reviews, which is typical of real-world review data.

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/your-username/sentiment-majitar.git
cd sentiment-majitar
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the model**
```bash
python model_fixed.py
```

---

## 📈 Sample Output

```
Naive Bayes Accuracy: 0.75

Naive Bayes Report:
              precision    recall  f1-score   support
    negative       0.00      0.00      0.00         0
     neutral       0.00      0.00      0.00         1
    positive       0.75      1.00      0.86         3

Custom Predictions:

Review    : Food was amazing and service was great
  NB Pred : positive
  LR Pred : positive

Review    : Worst food ever and rude staff
  NB Pred : negative
  LR Pred : positive

Review    : Food was okay but expensive
  NB Pred : negative
  LR Pred : positive
```

---

## ⚠️ Limitations

- Only 20 reviews — results are for academic demonstration
- Class imbalance (more positives than negatives/neutral)
- Classical models used; BERT/transformers would perform better on larger data
- No stopword removal or lemmatization applied (kept beginner-friendly)

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **pandas** — data handling
- **scikit-learn** — TF-IDF, models, evaluation metrics
- **re** (built-in) — text cleaning

---

## 📚 References

- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- Manning, Raghavan & Schütze — *Introduction to Information Retrieval*
- Salton & Buckley (1988) — *Term-weighting approaches in automatic text retrieval*

---

## 👨‍💻 Author

**RAJDEEP DEY** · Register No: - 202300325  
B.Tech — Computer Science & Engineering  
Course: Natural Language Processing | 2023-2027
Sikkim Manipal Institute of Technology
Majitar, East Sikkim, India
