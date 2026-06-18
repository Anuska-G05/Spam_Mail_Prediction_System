# 📧 Spam Mail Prediction System

A Machine Learning and Natural Language Processing (NLP) project that classifies SMS messages as **Spam** or **Ham (Legitimate)** using **TF-IDF Vectorization** and **Logistic Regression**.

The project demonstrates a complete text-classification pipeline, including data preprocessing, feature extraction, model training, evaluation, and prediction on custom messages.

---

## 🚀 Project Overview

Spam messages are one of the most common forms of unwanted communication. This project uses Machine Learning techniques to automatically identify whether a message is spam or legitimate.

The system converts raw text into numerical feature vectors using **TF-IDF (Term Frequency–Inverse Document Frequency)** and trains a **Logistic Regression** classifier to detect spam messages with high accuracy.

---

## 🎯 Objectives

- Detect spam SMS messages automatically.
- Apply Natural Language Processing techniques to text data.
- Convert textual data into machine-readable numerical features.
- Train and evaluate a machine learning classification model.
- Predict the category of new unseen messages.

---

## 📂 Project Structure

```text
Spam_Mail_Prediction_System/
│
├── Spam_Mail_Prediction_using_Machine_Learning.ipynb
├── mail_data.csv
├── README.md
│
└── outputs/
```

---

## 📊 Dataset Information

### Dataset

The dataset contains SMS messages labeled as:

- **Spam** → Unwanted promotional or fraudulent messages
- **Ham** → Legitimate messages

### Dataset Statistics

| Attribute | Value |
|------------|--------|
| Total Records | 5,572 |
| Features | 2 |
| Target Classes | Spam / Ham |

### Columns

| Column | Description |
|----------|-------------|
| Category | Label (Spam or Ham) |
| Message | SMS text content |

---

## 🛠 Technologies Used

### Programming Language

- Python

### Libraries

- NumPy
- Pandas
- Scikit-Learn

### Machine Learning

- Logistic Regression

### NLP

- TF-IDF Vectorization

---

## ⚙️ Machine Learning Pipeline

### 1. Data Collection

- Load SMS dataset using Pandas.
- Inspect data structure and quality.

### 2. Data Preprocessing

- Handle missing values.
- Convert categorical labels into numerical values.

Encoding:

```text
Spam → 0
Ham  → 1
```

### 3. Train-Test Split

Dataset is divided into:

- Training Data (80%)
- Testing Data (20%)

### 4. Feature Extraction

Raw text messages are transformed using:

```python
TfidfVectorizer()
```

TF-IDF helps identify important words while reducing the impact of frequently occurring common words.

### 5. Model Training

The model is trained using:

```python
LogisticRegression()
```

### 6. Model Evaluation

Performance is evaluated on:

- Training Data
- Testing Data

Metrics:

- Accuracy Score

### 7. Prediction

Users can provide a custom SMS message, and the model predicts:

```text
Spam Mail
```

or

```text
Ham Mail
```

---

## 🔍 Feature Engineering

### TF-IDF Vectorization

The text messages are converted into numerical feature vectors using:

```python
TfidfVectorizer(
    min_df=1,
    stop_words='english',
    lowercase=True
)
```

Benefits:

- Removes common English stop words.
- Converts text into weighted numerical features.
- Improves classification performance.

---

## 📈 Workflow

```text
SMS Message
      │
      ▼
Data Cleaning
      │
      ▼
Label Encoding
      │
      ▼
TF-IDF Vectorization
      │
      ▼
Logistic Regression
      │
      ▼
Spam / Ham Prediction
```

---

## 💡 Example Prediction

### Input

```text
Congratulations! You have won a free iPhone. Click here to claim now.
```

### Output

```text
Spam Mail
```

---

### Input

```text
Hey, are we still meeting at 6 PM today?
```

### Output

```text
Ham Mail
```

---

## 📚 Key Concepts Demonstrated

- Natural Language Processing (NLP)
- Text Classification
- Supervised Machine Learning
- Logistic Regression
- TF-IDF Vectorization
- Data Preprocessing
- Feature Extraction
- Model Evaluation
- Spam Detection Systems

---

## 🎓 Learning Outcomes

Through this project, the following concepts were implemented:

- Working with real-world text datasets
- Cleaning and preprocessing textual data
- Feature extraction using TF-IDF
- Binary Classification
- Logistic Regression implementation
- Accuracy evaluation
- Prediction on custom input data

---

## 🔮 Future Improvements

Possible enhancements include:

- Naive Bayes Classifier
- Random Forest Classifier
- XGBoost
- Deep Learning Models (LSTM, GRU)
- BERT-based Spam Detection
- Web Application using Streamlit
- REST API using FastAPI
- Model Deployment on Cloud Platforms

---

## 🤝 Contributions

Contributions, suggestions, and improvements are welcome.

Feel free to fork the repository and submit pull requests.

---

## 📜 License

This project is intended for educational and learning purposes.

---

## ⭐ If you found this project useful

Please consider giving the repository a star to support the project and future development.