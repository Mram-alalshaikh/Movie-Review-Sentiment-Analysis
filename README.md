#  Movie Review Sentiment Analysis using NLP

An end-to-end Natural Language Processing (NLP) project that classifies IMDB movie reviews into **positive** or **negative sentiment** using machine learning techniques.

---

##  Overview

This project builds a complete pipeline starting from raw, unstructured text to final sentiment predictions.

The objective is to automatically understand audience opinions from movie reviews — simulating human interpretation of language.

---

##  Dataset

* **Dataset:** IMDB Movie Reviews
* **Size:** 50,000 reviews
* **Distribution:** 50% Positive / 50% Negative (Balanced)
* **Source:** Kaggle
* 
💡 The balanced dataset ensures fair training without bias toward any class.

---

##  Pipeline

###  Text Preprocessing

* Remove HTML tags & URLs
* Remove special characters
* Convert to lowercase
* Tokenization
* Stop-word removal
* Lemmatization

---

### Feature Engineering

* **TF-IDF Vectorization**
* **N-grams (1–3)** to capture context

---

###  Model Training

* Logistic Regression
* Support Vector Machine (SVM)
* Neural Network (MLP)
* Naive Bayes

---

## Results

| Model               | Accuracy   | F1-Score  |
| ------------------- | ---------- | --------- |
| Logistic Regression | **89.46%** | **0.895** |
| SVM                 | 88.63%     | 0.886     |
| MLP                 | 87.13%     | 0.871     |
| Naive Bayes         | 86.37%     | 0.864     |

---

##  Feature Comparison

| Method       | Accuracy   |
| ------------ | ---------- |
| TF-IDF       | **89.47%** |
| Bag-of-Words | 86.85%     |

 **TF-IDF outperformed Bag-of-Words by +2.62%**

 This demonstrates that feature representation has a major impact on model performance.

---

##  Evaluation

* High True Positives & True Negatives
* Balanced errors (False Positives ≈ False Negatives)
* No bias toward any class

---

##  Model Stability (Cross-Validation)

* Mean CV Accuracy: **89.33%**
* Test Accuracy: **89.45%**
* Difference: **0.12%**

 The small gap confirms that the model generalizes well and does not overfit.

---

##  Limitations

* Struggles with sarcasm and irony
* Difficulty capturing negation (e.g., "not good")
* Mixed sentiment reviews create ambiguity

---

##  Future Work

* Multi-class sentiment classification (1–5 stars)
* Word embeddings (Word2Vec, GloVe)
* Transformer-based models (BERT, RoBERTa)

 These approaches can better capture contextual meaning and complex language patterns.

---

##  Project Structure

```
movie-review-sentiment-analysis/
│
├── notebook/
│   └── sentiment_analysis.ipynb
│
├── slides/
│   └── presentation.pdf
│
├── README.md
```

---

##  Presentation

 [View Slides](./slides/presentation.pdf)

---

##  Notebook

 [Open Notebook](./notebook/sentiment_analysis.ipynb)

---

##  Key Insight

> Feature engineering is a critical factor in NLP performance.
> TF-IDF significantly improves model accuracy by weighting informative words rather than treating all words equally.

---

##  Author

**Mram Alalshaikh**
Master’s Student in Data Science

---

## Support

If you found this project useful, feel free to ⭐ star the repository!
