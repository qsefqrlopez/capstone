# Capstone - Fake News Classifier
Authors: Quinton Lopez

## Problem Statement
---
To build a Natural Language Processing model that accurately classifies an article of news as real or fake.


With the increasing users on multiple social media platforms and political parties looking to gain advantages, fake news is more common than ever. This should be no surprise with the huge volume of data being generated from people all around the world. Dictionary.com listed 'misinformation' as the word of the year in 2018. Fake news is classified as news that has a false connection, false context, misleading, or fabricated content. In other words, fake news is any news that is factually wrong, misrepresents the facts, and spreads to targeted audiences. These instances of fake news is purposefully done with the intentions of pushing certains ideas to readers for a political or social influence, media manipulation, and financial profit. With the emergence of social media, not only does it spread through television and radio, but also outlets such as Facebook, Twitter, Reddit, etc. The lack of trust in the media is a growing problem that effects the democracy we live in as well as the way our society receives information. 


## Executive Summary
---
In this project, I collected a fake news dataset from a Kaggle Prediction Competition to build a CVEC & Multinomial Naive Bayes model that can accurately classify a news article as real or fake based on the text. My goal is to build a model that more accurately classifies news as real or fake better than the null model, plurality class.

My approach after collecting the dataset, was to clean and remove the null values as well as the columns besides the text and target. I was able to clean the article entries by using a variety of functions and transformers to remove special characters, tokenize, lemmatize, and remove less meaningful words.

Once the text data was pre-processed and I was able to visualize the data in my exploratory data analysis. To better understand the data, I created columns such as polarity and word count. I wanted to explore if there was a correlation between the sentiment of a real or fake article. I began testing multiple models and numerous hyperparameters to produce an accuracy score that outperforms the null model. 

## Contents of Repository
1.[Raw Data](https://git.generalassemb.ly/qrlopez/final/tree/master/data)

2.[Project Notebook](https://github.com/qsefqrlopez/capstone/blob/master/code/fake_news_code.ipynb)

3.[Presentation Slides](https://docs.google.com/presentation/d/1Tp-ckw-0JNRWawDvtnv__E5qXU0r37I74fVChnfKd_o/edit?usp=sharing)


## Data Dictionary
---
Column | Description
id | number of entry 
title | name of article 
author | writer of article 
text | the main body of the article or piece of writing
label | classification of article, 0 represents real and 1 represents fake
polarity | sentiment score of each article in the range of [-1,1], 1 means positive sentiment and -1 means a negative sentiment
length | total number of characters in a article
word count | total number of words in a article
label class | classification of article by True and False



## Conclusion & Recommendation
---
The model I have chosen, TFID and Logistic Regression, will accurately classify whether an article is real or fake based on the text. After cleaning and visualizing the data, along with  creating multiple models, I have come to this conclusion. In comparison with the other models, this outperforms them all and will give you the best accuracy to properly classify the article. This model should be applied before sharing any content with friends or on social media. 

It is important to fact check whenever you read an article or post. You should also choose to consume information from trusted sources that have multiple filters or must abide by a certain ethic code. It is just as important to be aware that certain main media sources have a news bias. They may be presenting the same information but from a different sentiment and perspective. Also consider not reading the headlines and passing information if you have not read the text. This is considered false connection and is intended to mislead consumers.


## References
---
1. [Data](https://www.kaggle.com/c/fake-news/data)
2. [Fake News](https://en.wikipedia.org/wiki/Fake_news)
3. [Global Lesson Classification Metric II](https://git.generalassemb.ly/DSI-US-12/4.05-lesson-classification-metrics-ii)
4. [Fake News & AI](https://miguelmalvarez.com/2017/03/23/how-can-machine-learning-and-ai-help-solving-the-fake-news-problem/)

