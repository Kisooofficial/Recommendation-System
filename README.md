# What is this repository?
This is a repository that I had practiced Instagram Crowling for sentiment analysis. 
# What kind of activity contains?
+ Instagram Crawling : Practice Python Crowling using BeautifulSoup and Selenium
+ Melon Crawling : Get 4000 songs from Melon Chart
+ Sentiment Analysis for single sentence (sentiment_analysis.ipynb)
=> apply machine learning model (LightGBM, Logistic Regression)
+ Sentiment Analysis for several sentence(same as dialogue) (sentiment_model_practice.ipynb)
=> using LSTM model
+ Recommendation System using sentiment analysis (참빛설계 학습모델 테스트 - 멜론 Top 100)

# What I used?
## Programming Language
+ Python Jupyter Notebook

## Library
+ Selenium
+ BeautifulSoup
+ Numpy
+ Pandas
+ Keras 
+ Konlpy
+ Tf-IDF 

### Data
+ AI Hub Data
+ Melon Song Information Data

## Modeling
|Model Name|Accuracy|
|---|---|
|Logistic Regression|17.36%|
|Random Forest|17.69%|
|LightGBM|18.04%|
|LSTM|68.05%|

## How to Recommend?
Since the accuracy was not high enough, cosine similarity was used to make a better recommendation.
+ sentiments are predicted using a model learned from the user's SNS posts and collected songs.
+ extract only the same of the predicted emotions from SNS and songs.
+ compare the extracted cosine similarity and recommend the top 5 songs with the highest similarity.
