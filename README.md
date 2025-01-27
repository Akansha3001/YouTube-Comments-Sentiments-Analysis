# YouTube Comments Sentiment Analysis

## Overview

This project leverages a Kaggle dataset of trending YouTube videos from the US and UK to perform comprehensive data analysis and sentiment evaluation. By exploring the relationship between video statistics, comments, and sentiment, the project aims to uncover patterns in user engagement and identify factors contributing to a video's popularity on YouTube.

## Objectives

Sentiment Analysis: Analyze the sentiment of comments (positive, negative, neutral) and visualize sentiment distribution.
Text Analysis: Examine comment lengths, word frequency, and generate word clouds for sentiment-specific and overall comments.
Statistical Analysis: Identify correlations between key features like likes, replies, and video views.
Predictive Modeling: Build machine learning models to classify comment sentiment based on text data.

## Dataset

The dataset was sourced from Kaggle, containing two key files:

### Video Statistics:

video_id: Unique identifier for videos (common field with the comments file).
title, channel_title, tags: Metadata about the video.
views, likes, dislikes: Engagement metrics.
category_id: Mapped to a category using JSON.
date: The date the video trended.

### Comments:

video_id: Unique identifier linking to the video file.
comment_text: Content of the user comment.
likes: Number of likes on the comment.
replies: Number of replies to the comment.
Dataset Link: https://www.kaggle.com/datasets/datasnaek/youtube

## Tools and Libraries

Python: Programming language used for analysis.
Pandas: For data manipulation and cleaning.
Matplotlib & Seaborn: For visualization.
WordCloud: For text visualization.
Scikit-learn: For building machine learning models.

## Key Steps in the Analysis

### Data Preprocessing:
Merged video statistics and comments files using the video_id field.
Cleaned and processed text data for analysis and modeling.

### Exploratory Data Analysis (EDA):
Visualized sentiment distribution using bar plots.
Analyzed comment lengths and generated histograms.
Created word clouds for positive, negative, neutral, and overall comments.
Analyzed correlations between numerical features like likes and replies.

### Sentiment Analysis Models:
Built and evaluated models to predict comment sentiment:
Naïve Bayes: Achieved an accuracy of 82%.
Gradient Boosting Classifier: Achieved an accuracy of 81%.

### Insights and Observations:

Neutral comments are the most frequent, followed by positive and negative.
Positive comments tend to be longer on average.
Significant correlation exists between likes and replies.
