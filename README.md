# reddit_data

|Table of Contents |
|---|
| [Overview](#overview) |
| [Data](#data) |
| [Key Insights](#key-insights) |

## Overview
This project is an exercise in webscraping and natural language processing and well as comparing random forests with other classifiers. The goal was to use data scraped from reddit to analyze which posts lead to higher user enagement, measured by number of comments. For this study, I classified the target into a binary variable - above or below median number of comments, with accuracy as the scoring metric.


## Data
HTML data was scraped from reddit (http://www.reddit.com). The web scraper retrieved data from the 'front page' of reddit and all following pages (there are 20 following pages). HTML data was then processed into key variables through feature selection and put into a pandas dataframe. Lastly, feature engineering was performed on the titles of the posts.

## Key Insights
Both the random forest and the logistic regression achieved accuracy scores in the low 70s, a certain improvement over the baseline of 50%. Part of the model tuning was the decision to include a countvectorizer. In this case, I do not believe the dataset has enough word data for the countvectorizer to be effective. For effective use of the countvectorizer, more data should be gathered, or the analysis should be performed on posts within a single subreddit (topic) where certain buzzwords and trends are more likely to exist.



## Concepts and Skills used
Python <br>
Pandas <br>
SKLearn <br>
BeautifulSoup <br>
Regex <br>
CountVectorizer <br>
Feature engineering <br>
Random Forest <br>
Logistic Regression <br>