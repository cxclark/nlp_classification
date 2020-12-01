# Subreddit Classification Using Language Processing

## Problem Statement: Which Subreddit?

Build a model to classify a subreddit post as belonging to either r/artificial or r/datascience, subreddits about artificial intelligence and data science, respectively. 

## Executive Summary

Subreddit post data was collected using the Pushshift API. The data is cleaned, features are engineered, and word trends are visualized.

The data is pre-processed, vectorized and modeled. Conclusions are drawn, and possible next steps are discussed.

## Conclusions

The optimal model for subreddit post classification was Logistic Regression with TfdifVectorizer. It achieved an accuracy score of 92.66% on the test data, with a recall score of 93.08% and a precision of 93.01%. The model was slightly overfit with a training accuracy of 97.85%.

The benefit of logistic regression is that interpretable word coefficients were able to be extracted and visualized. 

A performance boost was was observed when posts with missing text were dropped. This could be explained by more text conveying a stronger signal in an NLP model. It might also be the case that posts with title text only tended to be less relevant.

## Possible Next Steps
- Continue to test the model’s bias and variance by testing it on new data.
- Further validate the model on new posts.
- Explore other machine learning-related subreddits.

## Data Sources
1. [Artificial Intelligence Subreddit](https://www.reddit.com/r/artificial/)  
2. [Data Science Subreddit](https://www.reddit.com/r/datascience/)  