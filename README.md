# Sentiment_Analysis_using_Logisitic_Regression

This project implements sentiment analysis using **Logistic Regression**. It was developed as part of the Bachelor in Engineering (B.E.) curriculum, serving as the final year project.

## Project Overview

- **Objective**: Perform sentiment analysis on binary labeled data.
- **Steps**:
    1. **Data Cleaning**: Remove unnecessary and incorrect data points.
    2. **Stopword Removal**: Eliminate common stopwords.
    3. **Porter Stemming**: Apply Porter Stemmer to reduce words to their root form.
    4. **TF-IDF Vectorization**: Convert raw text documents into a matrix of TF-IDF features.
        - **TF-IDF (Term Frequency-Inverse Document Frequency)** assigns weights to each word based on its term frequency (TF) and inverse document frequency (IDF).
        - Equivalent to combining **CountVectorizer** (to count word occurrences) followed by **TfidfTransformer**.
    5. **Data Splitting**: Divide the data into 80% training and 20% testing sets.
    6. **Model Training and Testing**: Train the logistic regression model and evaluate its accuracy (achieved 89%).

## Usage

1. Clone this repository.
2. Install necessary dependencies (e.g., scikit-learn).
3. Run the provided Python script for sentiment analysis.


---

### About TF-IDF Vectorization

**TF-IDF Vectorization** (Term Frequency-Inverse Document Frequency) converts a collection of raw documents into a matrix of features. It is equivalent to combining **CountVectorizer** (which counts word occurrences) followed by **TfidfTransformer**. The process assigns weights to each word based on its term frequency and inverse document frequency, making it useful for text classification, information retrieval, and summarization.

### Porter Stemmer

The **Porter Stemmer** is a popular stemming algorithm proposed in 1980. It simplifies words by removing common morphological and inflectional endings, transforming them into their root form. While it's known for its speed and simplicity, it has limitations, such as occasionally producing non-words as root forms. In our project, we apply the Porter Stemmer to enhance text normalization.

