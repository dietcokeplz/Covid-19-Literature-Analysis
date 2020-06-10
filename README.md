# Covid-19-Literature-Analysis

For this project I analyze the literatures of Covid-19 from various sources using LDA topic modeling, and make recommendations based on similarities using collaborative filtering to the text that user put into the LDA model to find topic for.

My project is divided into the following tasks:

### I. Exploratory Data Analysis

Find out the distribution of articles within the dataset and provide a visual and descriptive statistics.

### II. Natural Language Processing and Topic Modeling

Utilize NLP techniques to preprocess the text: handling multiple languages, remove punctuations/stopwords, tokenize the text and other feature engineering. Apply LDA for topic modeling and grid search method is used to find the optimal hyperparameters combinations. 

### III. Content Based Collaborative Filtering : reformat the df dataframe to be shaped with papers as the rows and topics as the columns.

Each paper should only appear in each row once.<br>
Each topic should only show up in one column.<br>
I set the limit of number of topic to 3 so all the text that is put into LDA model to find topic will should only show as many as 3 topics with highest probability.<br>
If a paper has interacted with a topic, then place a 1 where the paper-row meets for that topic-column.<br>
If a topic does not show as one of the top 3 topics of a paper, then place a 0 where the paper-row meets for that topic-column

### IV. Topic Modeling the unseen text and Matrix Factorization

Unseen text that is put into lDA model will return the top 3 topics with highest probabilities.<br>
Generate a single row for the unseen text where the row stands for the paper and the columns represent all the topics. Place model returned probability under corresponding topic column and put 0 everywhere else.<br>
Build similarity matrix factorization to make paper recommendations. Paper with the highest similarities will be recommended to the unseen text.

### V. LDAvis visualization of LDA model topics

Unfortuanately, the visualization of the LDA model topics using LDAvis moduel is not able to be shown by Github currently.
The visualization should be similar to picture at the Url: https://stackoverflow.com/questions/32531031/calculate-intertopic-distances-from-ldavis-package, which gives a more precise idea on how the papers distributed and what are the most salient terms in every topic.
