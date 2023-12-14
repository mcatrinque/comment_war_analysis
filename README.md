# International Conflicts Sentiment Analysis

## Introduction

This project aims to analyze discourses and predict whether the discourse expresses war support, war opposition, or is neutral, specifically related to the Israel-Palestine and Russia-Ukraine conflicts.

## Data Preparation

### Loading and Consolidating Datasets

The data preparation phase involves consolidating information related to the conflicts. Two datasets, 'ukr_rus_reddit_comments.csv' and 'isr_pse_reddit_comments.csv', are loaded and unified into a DataFrame named `conflict_war_df`.

## Text Preprocessing

### Preprocessing Text Data

Before sentiment analysis, text preprocessing is crucial. This includes removing punctuation, tokenization, removing stopwords, and lemmatization.

## Sentiment Analysis

### Analyzing Sentiments with NLTK

The NLTK's `SentimentIntensityAnalyzer` is used to classify sentiments into war support, war opposition, or neutral categories. It provides compound, positive, neutral, and negative scores.

## Data Preparation for Model

### Encoding and Tokenization

The data is prepared for model training by encoding labels, splitting into training and testing sets, and tokenizing the text data.

## Model Training

### Building and Training the Model

A deep learning model is constructed using an embedding layer, bidirectional LSTM layer, and a dense layer. Class weights are balanced for handling class imbalances.

## Results

### Model Evaluation and Analysis

The model's performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. Additionally, sentiment counts and visualizations are presented for further analysis.

## Conclusion

Based on the training results and sentiment analysis, the model demonstrates promising performance in classifying sentiments related to conflicts. Further analysis, visualizations, and metrics provide insights into the model's effectiveness.

## Future Work

A potential future enhancement could involve extending the analysis to predict the specific country (Ukraine, Russia, Israel, Palestine) to which a given comment tends.

## Contributions Produced

The final dataset, `conflict_war_df`, is saved to 'conflict_war_df.csv'. The dataset includes columns such as 'post_id', 'comments', 'conflict', and 'sentiment'.

## References

- [Israel Palestine War Sentiment Analysis](https://www.kaggle.com/code/shamsheerrahiman/israel-palestine-war-sentiment-analysis/)
- [Ukraine Russia War Reddit Data](https://www.kaggle.com/datasets/diyacharya/ukraine-russia-war-reddit-data)
```
