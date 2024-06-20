# Hate Speech Detection in Movie Reviews

## Objective

Our objective as a hate speech detection system for movie reviews is to filter user-generated material, spotting and reporting offensive language. Our goal is to make the online movie-watching experience safer and more welcoming by utilizing machine learning techniques and text data analysis.

## Dataset

The dataset used for this project can be found at the following URL:
[Hate Speech and Offensive Language Dataset](https://github.com/t-davidson/hate-speech-and-offensive-language/blob/master/data/labeled_data.csv)

## Instructions

### 1. Data Cleaning

The `data_cleaning.py` script is responsible for:
- Loading the raw dataset.
- Expanding abbreviations using the `abbreviations.py` module.
- Cleaning the text data by removing unwanted characters, punctuation, and stopwords.
- Saving the cleaned data to `cleaned_data.csv`.

### 2. Tokenization and Encoding

The `encoding.py` script handles:
- Loading the cleaned dataset (`cleaned_data.csv`).
- Tokenizing the text data.
- Applying TF-IDF encoding to the tokenized data.
- Saving the TF-IDF encoded data to `tfidf_encoded_data.pkl`.
- Evaluating the accuracy using a Random Forest classifier.

## Results

- **Model Accuracy**: The Random Forest classifier achieved an accuracy of 89.69%.