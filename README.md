# Tweet-classification
## Project objective
The goal of this project is to classify text on a social network (in this case, twitter/X, in order to prevent influencing the audience in the run-up to the elections). The text of the tweets will be classified and, if necessary, the user will be banned/informed about the prohibition of these statements.
The main quality metric will be the F1 score - since the task will be multi-class classification of text in which there is an imbalance of classes, this metric will most fully reflect the quality of the model.
## Analysis and data
In this area, there are solutions using both classical machine learning algorithms (https://habr.com/ru/articles/677512/) and using pre-trained neural networks (https://neurohive.io/ru/tutorial/bert-klassifikacya -teksta/). In classical machine learning, both logistic regression (as in the article) and gradient boosting are widely used. These algorithms show good results (accuracy = 65%) and are still quite capable of being used in business tasks. Neural networks show much better results, especially pre-trained models (accuracy = 99%). In this work we will compare these algorithms and verify the conclusions.
In our work, we downloaded 4 parts of the original data set, resulting in 984,107 rows and 21 columns with a description of the tweets themselves, as well as information about users.
The data was taken from the following repository https://github.com/fivethirtyeight/russian-troll-tweets;
The data is presented in .csv format;
The dataset contains data from tweets sent from Twitter accounts associated with the Internet Research Agency, a Russian troll factory, and a defendant in the Justice Department's February 2018 indictment as part of special counsel Robert Mueller's Russia investigation. Tweets in this database were sent between February 2012 and May 2018, with the vast majority posted from 2015 to 2017;
For this work, a dataset of 984,107 rows and 21 columns was compiled;
The dataset contains 8 classes of tweets in 51 languages.
