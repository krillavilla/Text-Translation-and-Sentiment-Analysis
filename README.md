Definitely! Here's your `README.md` in **pure markdown format**, ready to be dropped directly into your GitHub repo:

---

# 🎬 Multilingual Movie Review Sentiment Analysis with Transformers

## 🧠 Project Overview

This project analyzes movie reviews written in **English, French, and Spanish**, translating non-English content and determining whether the review sentiment is **Positive** or **Negative** — all using **pre-trained transformer models** from HuggingFace 🤗.

We combined **Natural Language Processing (NLP)**, **data preprocessing**, and **machine learning workflows** to produce a unified, language-normalized dataset and analyze sentiments across 30 international films.

---

## 🗂️ Final Output

A single CSV file with the following columns:

- **Title**
- **Year**
- **Synopsis** (translated to English if necessary)
- **Review** (translated to English if necessary)
- **Sentiment** (Positive / Negative)
- **Original Language** (`en` / `fr` / `sp`)

✅ Each of the 30 rows corresponds to a unique movie and includes fully translated and analyzed reviews.

---

## 🚀 Features & Workflow

### ✅ Step 1: Data Ingestion
- Loaded and merged three CSV files:
  - `movie_reviews_eng.csv`
  - `movie_reviews_fr.csv`
  - `movie_reviews_sp.csv`
- Created a single, clean DataFrame with consistent columns.

### 🌍 Step 2: Language Translation
- Identified non-English reviews and synopses.
- Translated **French** and **Spanish** texts to English using HuggingFace transformer models:
  - `Helsinki-NLP/opus-mt-fr-en`
  - `Helsinki-NLP/opus-mt-es-en`

### 💬 Step 3: Sentiment Analysis
- Used a pre-trained sentiment analysis model:
  - `distilbert-base-uncased-finetuned-sst-2-english`
- Generated **Positive** or **Negative** sentiment labels for each review.

---

## 🛠️ Tools & Libraries

| Tool                  | Usage                                |
|-----------------------|--------------------------------------|
| `Pandas`              | Data loading and preprocessing       |
| `HuggingFace Transformers` | Translation & Sentiment Analysis |
| `PyTorch`             | Backend for transformer models       |

---

## 🧠 Skills Demonstrated

- Multilingual NLP pipeline construction
- Data cleaning and preprocessing with Pandas
- Text translation using transformer models
- Sentiment classification using fine-tuned BERT models
- Integration of multiple ML/NLP tools into a cohesive solution

---

## 📁 Project Structure

```
.
├── data/
│   ├── movie_reviews_eng.csv
│   ├── movie_reviews_fr.csv
│   └── movie_reviews_sp.csv
├── notebooks/
│   └── analysis_pipeline.ipynb
├── src/
│   ├── data_loader.py
│   ├── translator.py
│   └── sentiment.py
├── output/
│   └── translated_sentiment_reviews.csv
├── README.md
└── requirements.txt
```

---

## 📈 Future Improvements

- Deploy as a Streamlit web app for live translation and sentiment scoring
- Add language detection for more robust preprocessing
- Expand language support to include German, Italian, Japanese, etc.

---

## 🙌 Acknowledgments

- [HuggingFace](https://huggingface.co/) for providing powerful transformer models
- Udacity for the NLP project framework and inspiration

---

## 📫 Connect

**Author**: Kashad Turner-Warren  
**LinkedIn**: [linkedin.com/in/kashadturnerwarren](https://linkedin.com/in/krillavilla)  
**GitHub**: [@krillavilla](https://github.com/krillavilla)

---

