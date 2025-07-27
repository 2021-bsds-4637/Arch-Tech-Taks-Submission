
# 📧 Email Spam Detection with Machine Learning

This project uses Natural Language Processing (NLP) and machine learning to classify emails as **spam** or **not spam**. It involves text preprocessing, feature extraction, model training, and evaluation using multiple classifiers.

---

## 📂 Dataset

- **Source**: A CSV file containing email content and spam labels.
- **Columns**:
  - `text`: Raw email content (subject + body)
  - `spam`: Target label (1 = spam, 0 = not spam)

---

## 🔍 Project Workflow

### 1. Text Preprocessing
Applied standard NLP preprocessing to the `text` column:
- Lowercasing
- Removing punctuation and numbers
- Removing stopwords
- Tokenization
- Lemmatization (WordNetLemmatizer)

### 2. Feature Extraction
Used **TF-IDF Vectorization** to convert preprocessed text into numerical vectors:
```python
TfidfVectorizer(max_features=1000)
```

### 3. Train-Test Split
Split the dataset using `train_test_split()`:
- 80% training
- 20% testing
- Stratified by target label

### 4. Model Training
Trained four different classifiers:
- ✅ Logistic Regression
- ✅ Multinomial Naive Bayes
- ✅ Random Forest
- ✅ Support Vector Machine (SVM - LinearSVC)

### 5. Model Evaluation
Evaluated models using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix (with plots)

---

## 📈 Sample Output

| Model                 | Accuracy | Precision | Recall | F1 Score |
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  | 0.97     | 0.95      | 0.98   | 0.96     |
| Multinomial NB       | 0.96     | 0.93      | 0.97   | 0.95     |
| Random Forest        | 0.95     | 0.91      | 0.96   | 0.93     |
| SVM (LinearSVC)      | 0.97     | 0.96      | 0.97   | 0.96     |

> *(Scores are illustrative – replace with your actual results.)*

---

## 🚀 How to Run

1. Clone the repository or download the notebook.
2. Place your `emails.csv` file in the project directory.
3. Run the notebook or Python script to:
   - Preprocess data
   - Train models
   - Evaluate performance

---

## 🛠 Dependencies

Make sure to install these before running the project:

```bash
pip install pandas numpy scikit-learn matplotlib nltk
```

Also run the following once to download NLTK resources:

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```

---

## ✨ Future Improvements

- Add word cloud or top spam word visualization
- Try deep learning with LSTM or BERT
- Deploy using Flask or Streamlit for live predictions

---

