# Group-8-Final-Project
Project Name: Course Recommendations with Machine Learning
Project Overview: We used natural language processing (NLP) to build a machine learning program that identifies and recommends relevant courses based on the user’s input.
Data Set Source: Course Relevance Dataset from Kaggle
Machine Learning Tools: 
PySpark
Matplotlib
Pandas
NLTK
Tokenizer
Lemmatizer (Lemmatization is the pre - process involved in natural language processing, which involves distilling words to their foundational forms)
Stop words
Sklearn
TF-IDF (TF-IDF essentially combines TF and IDF to give a balanced score. It’s a technique to quantify important or rare words that appear frequently in documents)
Nearest Neighbor

Data Model Preparation and optimization : Created a new column ‘Robust’ by combining 3 other columns to enhance the search function. Checked for missing values in the dataset. Used WordNetLemmatizer() to convert the robust description to their basic word forms. And used TfidfVectorizer() to convert the text data into numerical vectors.
Limitation and Future Development: Based on the data fed i.e course description into the model, it will pick up results that might not necessarily relate to the course you’re looking for as a whole. In the future, the code should adapt to new data or user interactions over time to make the results more accurate to the course that the user is looking for. Build a user-friendly interface for inputting searches and viewing recommendations using Flask. Part of speech could be incorporated in the Lemmatizer, providing more accuracy to Lemmatized words.
Ethical Consideration: Bias and Fairness, Privacy and Consent and Misuse and Manipulation
 
