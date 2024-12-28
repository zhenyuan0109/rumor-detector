# Chinese Social Media Text Analysis Project

## Introduction
This project is focused on analyzing and classifying text data from Chinese social media posts to determine if a post is a rumor or not. The analysis involves text preprocessing, word segmentation using Jieba, stopword removal, word frequency analysis, and word cloud visualization, followed by the application of Naive Bayes classifiers for text classification.

## Dataset Description
The dataset contains social media posts in Chinese, each labeled as a rumor or not. The data is preprocessed to remove empty entries and transform content into a list format for further processing.

## Objective
The main objective is to develop a model that can accurately classify posts as rumors or not based on their content.

## Methodology

### Data Preparation
- **Data Loading**: Social media posts are loaded and preprocessed using pandas.
- **Text Segmentation**: Posts are segmented into individual words using Jieba.
- **Stopword Removal**: Common stopwords are removed to clean the text data.

### Data Analysis
- **Word Frequency Calculation**: Calculate the frequency of each word in the dataset.
- **Word Cloud Visualization**: Visualize the most frequent words using a word cloud.

### Model Training and Testing
- **Feature Engineering**: Use `CountVectorizer` and `TfidfVectorizer` for word embedding.
- **Model Building**: Train a Naive Bayes classifier to predict whether a post is a rumor.
- **Model Evaluation**: Evaluate the model's performance on a test set.

## Requirements
To run this project, you will need:
- Python 3
- pandas
- jieba
- matplotlib
- sklearn
- wordcloud
- zipfile

## Usage
Instructions on how to execute the project:
1. Extract the dataset using Python's `zipfile` module.
2. Load and preprocess the data.
3. Perform text analysis and visualization.
4. Train and evaluate the Naive Bayes classifiers.

## Results
The performance of the model can be measured by its accuracy in classifying posts correctly. Results include a comparison between using `CountVectorizer` and `TfidfVectorizer`.

## Contributors
- Zhenyuan Ni

## Additional Notes
- Ensure that the Chinese font path is correctly specified for the word cloud to display Chinese characters properly.
- Adjust the `max_features` parameter in vectorizers to balance between performance and computational efficiency.

