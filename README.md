# Natural-Language-Processing-with-Disaster-Tweets

-Performed EDA on twitter data and text classification of tweets into Disaster and Non-Disaster tweets.

-Detecting patterns in the tweet and classify using various machine learning models to achieve F1 score of 80.3%.

-Performed Sentiment analysis on twitter data using Multinomial Naïve Bayes using Count vectorizer.

# Pipeline and Methods

We imported required libraries and set random seed. We used the seed() method to customize the start number of the random number generator. For Exploratory Data Analysis, we loaded the data and checked for null values. Then, we investigated features such as "keywords", "location", and "tweet". Next, we created visualizations such as bar plots and histograms to understand the data. For Data Preprocessing, we wrote several functions for different tasks such as for removing URLS, removing non printable characters, removing all english stopwords, etc.

For Vectorizing the train and test data we used count vectorizer to convert a collection of text documents to a matrix of token counts. For vectorizing the train and test data, we also used Tfit vectorizer to convert a collection of raw documents to a matrix of TF-IDF features. 

For creating different models [LogisticRegression, SVC, MultinomialNB, DecisionTreeClassifier, KNeighborsClassifier, RandomForestClassifier] to compare results, we assigned the random state. A random_state parameter may be provided to control the random number generator used.  For each model, we used both vectorizers (count and tfidf) to fit and predict. Then we printed the model,  vectorizer, F1 score, and accuracy (training and testing) in descending order. Multinomial Naive Bayes with count vectorizer resulted in the best F1 score. We used Multinomial Naive Bayes with count vectorizer to create the submission file.


# Training Performance

![image](https://user-images.githubusercontent.com/71151379/120144361-c2688780-c1af-11eb-9bd6-1d01436039b8.png)

# Final testing performance and ranking in Public Leaderboard

Final testing performance - 0.79619

Ranking in Public Leaderboard - 1232

