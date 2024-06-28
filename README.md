# Group-8-Final-Project

## Project Name
Course Recommendations with Machine Learning

## Authors
- Cataldo Cocuzza
- Adrian Dayrit
- Kefan Liao
- Fay Muhammad
- Robert Rose
- Christopher Scarlata

## Project Overview
We used natural language processing (NLP) to build a machine learning program that identifies and recommends relevant courses based on the user’s input.

## Dataset Source
'Course Relevance Dataset' from [Kaggle] (https://www.kaggle.com/datasets/prasad22/course-relevance-dataset)
Total data points n = 905

| Data Attributes         | Description                                              | Data Type |
|-------------------------|----------------------------------------------------------|-----------|
| SrNo                    | Serial Number                                            | Integer   |
| Name Of the Program     | Graduation or Post Graduation Program                    | String    |
| Type of Course          | Subject Name within selected program                     | String    |
| Code                    | Subject Code                                             | String    |
| Need                    | Type of Developmental Need the subject is catering to    | String    |
| Description of the need | Description of Developmental Need associated to the subject | String |


## Machine Learning Tools 
- **PySpark**
- **Matplotlib**
- **Pandas**
- **NLTK**
- **Tokenizer**
- **Lemmatizer** (Lemmatization is the pre - process involved in natural language processing, which involves distilling words to their foundational forms)
- **Stop words**
- **Sklearn**
- **TF-IDF**
 - Term Frequency (TF) – Measures how often a word appears in a document, with more frequent words getting higher scores.
 - Inverse Document Frequency (IDF) – Highlights unique words by lowering the score of common words.
 - TF-IDF essentially combines TF and IDF to give a balanced score. It’s a technique to quantify important or rare words that appear frequently in documents
- **Nearest Neighbor**

## Data Model Preparation and Optimization
1. Created a new column ‘Robust’ by combining 3 other columns to enhance the search function.
2. Checked for missing values in the dataset.
3. Used WordNetLemmatizer() to convert the robust description to their basic word forms.
4. Used TfidfVectorizer() to convert the text data into numerical vectors.

## Limitation and Future Development
### Limitations
Based on the data fed i.e course description into the model, it will pick up results that might not necessarily relate to the course you’re looking for as a whole. 
### Future Development
In the future, the code should adapt to new data or user interactions over time to make the results more accurate to the course that the user is looking for. Build a user-friendly interface for inputting searches and viewing recommendations using Flask. Part of speech tagging could be incorporated in the Lemmatizer, providing more accuracy to Lemmatized words.

## Ethical Consideration
Bias and Fairness, Privacy and Consent and Misuse and Manipulation. No ethical concerns for this project
