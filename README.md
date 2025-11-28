# Tweet Virality Prediction (Machine Learning + Streamlit)

This project uses **machine learning** to predict whether a tweet is likely to go viral.  
Tweet text is processed using **CountVectorizer and TF-IDF**, and a **Naive Bayes classifier** is trained to identify patterns behind tweet popularity.

After testing both approaches, the **CountVectorizer + Naive Bayes** model achieved the best overall performance.

---

##  Features

- Text vectorization using **CountVectorizer** and **TF-IDF**
- Naive Bayes classification model
- Data cleaning & preprocessing
- **Streamlit web application**
- Real-time tweet virality prediction
- Prediction confidence score

---

##  Technologies Used

- Python
- Pandas
- Scikit-Learn
- CountVectorizer
- TF-IDF Vectorizer
- Naive Bayes
- Streamlit
- Joblib

---

##  Model Performance

Two models were tested:

| Vectorizer | Accuracy | Viral Recall | Viral Precision |
|----------|----------|---------------|----------------|
| **CountVectorizer** | **88%** | **98%** | 73% |
| TF-IDF | 83% | 46% | **95%** |

The **CountVectorizer + Naive Bayes** model was chosen for the Streamlit web app due to its high ability to correctly identify viral tweets.

---

##  How to Run the Web App

Make sure Python is installed, then run:

```bash
pip install streamlit joblib scikit-learn pandas
python -m streamlit run app.py
