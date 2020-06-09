# Covid-19-Literature-Analysis

For this project I analyze the literatures of Covid-19 from various sources using LDA topic modeling, and make recommendations based on similarities using collaborative filtering to the text that user put into the LDA model to find topic for.

My project is divided into the following tasks

I. Exploratory Data Analysis

Find out the distribution of articles within the dataset and provide a visual and descriptive statistics.

II. Natural Language Processing and Topic Modeling

Utilize NLP techniques to preprocess the text: handling multiple languages, remove punctuations/stopwords, tokenize the text and other feature engineering. Apply LDA for topic modeling and grid search method is used to find the optimal hyperparameters combinations. 

III. Content Based Collaborative Filtering : reformat the df dataframe to be shaped with papers as the rows and topics as the columns.

Each user should only appear in each row once.
Each article should only show up in one column.
If a user has interacted with an article, then place a 1 where the user-row meets for that article-column. It does not matter how many times a user has interacted with the article, all entries where a user has interacted with an article should be a 1.
If a user has not interacted with an item, then place a zero where the user-row meets for that article-column
V. Matrix Factorization Build use matrix factorization to make article recommendations to the users on the IBM Watson Studio platform
