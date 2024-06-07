The dataset has been successfully cleaned using clean_dataset.ipynb


Here are the steps we were performed:

1. Loaded the dataset.
2. Inspected the dataset: Confirmed it contains 24,783 rows and 7   columns with no null values.
3. Removed null values: No null values were found, so this step had no effect.
4. Removed duplicate rows.
5. Converted text in the 'tweet' column to lowercase.
6. Removed leading and trailing whitespaces in the 'tweet' column.
7. Removed special characters from the 'tweet' column.



additi_processing.ipynb


The code performs the following additional cleaning steps:

1. Tokenization: The text is split into individual words.
2. Stop Words Removal: Common words that do not add significant meaning are removed.
3.  Stemming: Words are reduced to their root form using PorterStemmer.
4. Lemmatization: Words are reduced to their base form using WordNetLemmatizer.