# 💬 Sentiment Analysis on Kaggle Dataset

This project aims to train and evaluate a sentiment prediction model using textual data collected from Kaggle. The goal is to preprocess the data, extract meaningful features, and build a reliable classifier capable of determining whether a message is **positive**, **negative**, or **neutral**.

📅 **Academic Year:** 2024 / 2025  
🎓 **Student:** Mohammed DECHRAOUI  
🏫 **Program:** M2SI — Master in Information Systems and Intelligent Systems  
📘 **Module:** Knowledge Discovery 1 & Text Mining  
📌 **Project Type:** Devoir Obligatoire  

---

## 🧠 Objective

Train a sentiment analysis model capable of predicting the sentiment of a given text using real-world data.

---

## 📂 Dataset

- **Train Set**: [`abhi8923shriv/sentiment-analysis-dataset`](https://www.kaggle.com/datasets/abhi8923shriv/sentiment-analysis-dataset)
- **Test Set**: [`guisira/cu-cedt-sentiment-analysis-testset`](https://www.kaggle.com/datasets/guisira/cu-cedt-sentiment-analysis-testset)
- Final dataset contains **27,480 samples**, after merging and cleaning.

---

## 🧹 Data Preprocessing Steps

1. **Data Loading** with `kagglehub`
2. **Merging & Filtering** (retaining only `text` and `sentiment`, and removing nulls)
3. **Stopwords Removal** using `NLTK`
4. **Tokenization** using `WordPunctTokenizer`
5. **Stemming** with `PorterStemmer`
6. **Vectorization** with `CountVectorizer (max_features=5000)`
7. **Label Encoding** using `LabelEncoder`
8. **Dataset Split**: 80% train / 20% test

---

## 📊 Exploratory Analysis

- Word frequency visualized using a **colored word cloud**
- Sample before/after text cleaning:
  
| Raw Text | Cleaned Text |
|----------|---------------|
| I`d have responded, if I were going | respond go |
| Sooo SAD I will miss you here in San Diego!!! | sooo sad miss san diego |

---

## 🤖 Model Training

- **Model Used:** Multinomial Naive Bayes (`MultinomialNB`)
- **Evaluation Metrics:**
  - Accuracy: **63.5%**
  - Classification Report (Precision, Recall, F1-score)
  - Confusion Matrix

---

## 🔎 Evaluation on Real Examples

```python
examples = [
  "I hate this product, it’s a complete disaster.",
  "This is fantastic, I highly recommend it!",
  "Not bad at all, but I expected better quality.",
  "I absolutely love it, works perfectly every time!",
  "Terrible experience, I will never buy this again."
]
```
## 🧪 Predicted Sentiments

- Negative  
- Positive  
- Neutral  
- Positive  
- Negative  

---

## 🚀 How to Run

1. **Clone the repo:**

```bash
git clone https://github.com/Mohammed78-Dch/sentiment-analysis.git
cd sentiment-analysis
```
---
## 🛠️ Tools & Libraries

- Python (Jupyter)
- Pandas, NumPy
- NLTK, SpaCy
- Scikit-learn
- WordCloud, Matplotlib
- KaggleHub

---

## 📈 Results

- Built a complete pipeline for **sentiment classification**
- Achieved over **63% accuracy** on real-world tweets and comments
- Validated predictions on **new textual examples**

---

## 📬 Contact

For inquiries or suggestions:

**Mohammed Dechraoui**  
📧 [mdechraoui@insea.ac.ma](mailto:mdechraoui@insea.ac.ma)  
🔗 [LinkedIn – Mohammed Dechraoui](https://www.linkedin.com/in/mohammed-dechraoui)

---

_This project was conducted as part of the **"Knowledge Discovery 1 & Text Mining"** module under the **M2SI** program at **INSEA**._

