# Hate Speech Detection in Movie Reviews

## Daniel Suresh

---

### 1. Business Problem
Hate speech in online movie reviews creates a toxic environment. It discourages participation and harms individuals. Identifying and moderating hate speech is crucial for maintaining a healthy online community.

---

### 2. Solution
We developed an AI model to detect hate speech in movie reviews. This automated moderation process helps create safer and more inclusive online platforms.

---

### 3. Dataset Description
- **Dataset**: [Davidson dataset](https://github.com/t-davidson/hate-speech-and-offensive-language/blob/master/data/labeled_data.csv)
- **Contents**: 24,000+ tweets classified as:
  - 0: Hate speech
  - 1: Offensive language
  - 2: Neither
- **Train and Test Data Split**:
  - **Train Data Size**: 19,826 samples
  - **Test Data Size**: 4,957 samples
  - **Split Ratio**: 80% train, 20% test

---

### 4. Data Visualization
To focus more on hate speech detection, we mapped offensive and hate speech to the same class:

- **Hate Speech (Class 0)**: 83.2%
- **Non-Hate Speech (Class 1)**: 16.8%

Class weights were used during model training to address the imbalance in the dataset.

---

### 5. Data Preprocessing
- Removed usernames, sequences, URLs
- Converted to lowercase
- Removed punctuations
- Replaced words (abbreviations, misspellings)
- Removed stopwords
- Lemmatization

Dataset after Data-Preprocessing : [cleaned_data.csv](https://drive.google.com/file/d/1YlA1XjLIHsaXA3AFmHjAeao3oHJUtYF4/view?usp=drive_link)

---

### 6. Tokenization and Embedding Techniques
#### 6.1 Tokenization Techniques
Used Keras Tokenizer to convert text into sequences.

#### 6.2 Embedding Techniques Considered
- **One-Hot Encoding**: Rejected (didn't capture semantic relationships)
- **TF-IDF**: Explored but less effective
- **GloVe**: Selected for capturing semantic meanings and relationships

**Why GloVe?**
- Pre-trained embeddings on a large corpus
- Captured semantic relationships crucial for hate speech detection

---

### 7. Modeling
#### 7.1 Machine Learning Models
- **Support Vector Machine (SVM)**: Explored but not selected
- **Logistic Regression**: Explored but not selected
- **Random Forest Classifier (RFC)**: Explored but not selected

#### 7.2 Deep Learning Models
- **Convolutional Neural Network (CNN)**: Explored but not selected
- **Bi-Directional LSTM**: Explored but not selected
- **LSTM with Attention**: Selected for final model

**Reasons for Model Selection**
- **LSTM with Attention**: Best balance of accuracy and efficiency, focusing on important parts of the text

---

### 8. Evaluation Metrics
- **Accuracy**: Overall correctness of the model
- **F1 Score**: Balanced precision and recall
- **Confusion Matrix**: Detailed breakdown of model performance

**Best Scores Achieved**
- **Deep Learning (LSTM with Attention)**
  - **Accuracy**: 91.04%
  - **F1 Score**: 91.65%

