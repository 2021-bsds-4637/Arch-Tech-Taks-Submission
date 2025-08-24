
# 🌸 Iris Flower Classification

This project is a beginner-friendly machine learning task using the famous Iris dataset. The goal is to classify iris flowers into three species — **Setosa**, **Versicolor**, and **Virginica** — based on their petal and sepal measurements.

---

## 📁 Dataset
- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/iris)
- Features:
  - SepalLengthCm
  - SepalWidthCm
  - PetalLengthCm
  - PetalWidthCm
- Target: Species (Setosa, Versicolor, Virginica)

---

## 📌 Objectives
- Perform data preprocessing and cleaning.
- Explore the dataset using visualizations.
- Train a classification model using **Random Forest**.
- Evaluate the model using accuracy, classification report, and confusion matrix.

---

## 🛠️ Libraries Used
- `pandas` – for data handling
- `seaborn` and `matplotlib` – for data visualization
- `scikit-learn` – for model building and evaluation

---

## 📊 Exploratory Data Analysis
- **Pairplot**: to observe the relationships between features by species.
- **Heatmap**: to analyze feature correlations.
- **Boxplots**: to understand feature distribution and class separability.

---

## 🤖 Model Building
- **Model Used**: `RandomForestClassifier` (from scikit-learn)
- **Train-Test Split**: 80% training, 20% testing
- **Evaluation Metrics**:
  - Accuracy Score
  - Classification Report (Precision, Recall, F1)
  - Confusion Matrix

---

## ✅ Results
- The model achieved **high accuracy**.
- **PetalLengthCm** and **PetalWidthCm** were the most important features for distinguishing species.
- `Setosa` was perfectly separable, while slight overlaps were observed between `Versicolor` and `Virginica`.

## 🚀 Future Enhancements
- Try different models: SVM, KNN, Logistic Regression
- Hyperparameter tuning with GridSearchCV
- Deploy using Streamlit for real-time predictions
