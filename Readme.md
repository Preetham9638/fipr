# 📈 Financial Market Sentiment Analysis

A machine learning project that predicts stock market movement (up/down) based on daily news headlines using Natural Language Processing (NLP) and a Random Forest Classifier.

---

## 📌 Project Overview

This project analyzes financial news headlines to determine whether the stock market will go **up (1)** or **down (0)** on a given day. It combines 25 news headlines per day into a single text feature, applies bag-of-words vectorization, and trains a Random Forest model to classify market sentiment.

---

## 🗂️ Dataset

- **Source:** [YBI Foundation – Financial Market News](https://raw.githubusercontent.com/YBI-Foundation/Dataset/main/Financial%20Market%20News.csv)
- **Format:** CSV with a `Label` column (0 = market down, 1 = market up) and 25 daily news headline columns
- **Encoding:** ISO-8859-1

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| Pandas & NumPy | Data manipulation |
| Scikit-learn | ML model, vectorizer, evaluation |
| Google Colab | Development environment |

---

## 🔄 Workflow

1. **Load Data** – Read CSV directly from GitHub URL
2. **Feature Engineering** – Concatenate 25 daily headlines into one text string per row
3. **Vectorization** – Apply `CountVectorizer` (unigrams, lowercase) to convert text to numeric features
4. **Train/Test Split** – 70% train / 30% test with stratification (`random_state=2529`)
5. **Model Training** – Random Forest Classifier with 200 estimators
6. **Evaluation** – Confusion matrix, classification report, accuracy score

---

## 🚀 How to Run

### On Google Colab
Click the badge below to open the notebook directly:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VyIrw_4aKnKm4wRghg9SovpwsgsqpmFs)

### Locally

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/financial-market-sentiment-analysis.git
cd financial-market-sentiment-analysis

# Install dependencies
pip install pandas numpy scikit-learn

# Run the script
python financial_sentiment.py
```

---

## 📊 Results

The model is evaluated using:
- **Confusion Matrix** – Visual breakdown of true vs predicted labels
- **Classification Report** – Precision, recall, F1-score per class
- **Accuracy Score** – Overall prediction accuracy

---

## 📁 Project Structure

```
financial-market-sentiment-analysis/
│
├── Financial_Market_Sentiment_Analysis.ipynb   # Main Colab notebook
├── financial_sentiment.py                      # (Optional) standalone script
└── README.md
```

---

## 🙋‍♂️ Author

Made with ❤️ as a beginner ML project.  
Feel free to fork, star ⭐, or raise issues!

---

## 📜 License

This project is open-source 
