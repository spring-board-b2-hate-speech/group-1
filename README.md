# group-1

Hate Speech Detection in Movie Reviews

Our objective as a hate speech detection system for movie reviews is to filter user-generated material, spotting and reporting offensive language. Our goal is to make the online movie-watching experience safer and more welcoming by utilizing machine learning techniques and text data analysis.

Dataset Description:- 
We used the Davidson dataset, a well-known source for hate speech research, for our hate speech detection project. Davidson et al.'s dataset includes over 24,000 annotated tweets classified as hate speech, offensive language, or neither, providing a well-balanced distribution for efficient model training and assessment. Its richness, diversity, and careful labeling make it ideal for developing robust algorithms to accurately identify offensive content in various contexts, including movie reviews.
dataset url : https://github.com/t-davidson/hate-speech-and-offensive-language/blob/master/data/labeled_data.csv

Data Preprocessing :-
To ensure our dataset is well-prepared for training and to enhance the quality and relevance of the text data, we undertook essential data cleaning and preprocessing steps. These measures systematically eliminate noise and standardize the dataset for analysis and model training:
 **Dataset Loading and Inspection:** Loaded the dataset and inspected its structure.
- **Usernames and Numeric Sequences Removal:** Removed usernames (mentions) and sequences of numbers.
- **URL Stripping:** Removed URLs to clean the text.
- **Text Lowercasing and Punctuation Removal:** Converted text to lowercase and removed punctuation marks.
- **Abbreviation Standardization:** Replaced common abbreviations and slang with their full forms.
- **Stopword Removal and Lemmatization:** Removed stopwords and lemmatized remaining words.

We used Visual studio for data cleaning and preprocessing. The preprocessing steps include tokenization, lemmatization, and normalization to prepare the dataset for training the model. These steps ensure that our dataset is clean, standardized, and optimized for hate speech detection tasks.
