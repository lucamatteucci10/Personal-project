# Twitter Sentiment Analysis - Final Deliverable

## Collaborators
- **Luca Matteucci**
- **Neeharika Kamireddy**
- **Haaniya Umair**
- **Sneha Jayapradeep**
- **Chirayu (Mitthi) Jain**

## Overview
This project aims to harness machine learning to automatically categorize sentiment in tweets as either positive or negative, which is crucial for understanding public sentiment on social media platforms like Twitter. The sheer volume of data on these platforms makes manual analysis impractical, necessitating automated methods to process and derive insights from such data.

## Problem Statement
Social media platforms are rich with public sentiment data that are pivotal in understanding prevailing attitudes. However, the vast amount of data makes manual analysis unfeasible. This project uses machine learning to categorize sentiment into positive or negative, uncovering deeper insights into the dynamics of sentiment expressed on social media.

## Dataset
The dataset is sourced from Stanford CS Datasets and contains tweets collected from April to June 2009. It includes 1.6 million rows across six columns: Polarity, Serial Number, DateTime, No_Query, Username, and Tweet Content. This dataset facilitates the exploration of unsupervised machine learning techniques to uncover inherent sentiment groupings.

## Exploratory Data Analysis (EDA)
- **Initial Examination**: Utilization of Python functions like `head()`, `isnull()`, and `describe()` to gauge dataset dimensions, missing values, and duplicates.
- **Visualizations**: Creation of graphs to display behavior of top Twitter users and a plot to exhibit the distribution of sentiments.
- **Observations**: An even distribution of positive vs. negative tweets, suggesting potential biases where neutral tweets might be misclassified.

## Preprocessing
- **Text Cleaning**: Conversion of text to lowercase and removal of non-alphanumeric characters, including punctuation and URLs.
- **Stop Words Removal**: Employment of NLTK's TweetTokenizer to enhance the quality of tokenized data.
- **Stemming and Lemmatization**: Standardization of word forms to reduce dimensionality and improve analysis efficiency.
- **Emoji Inclusion**: Retention of old school emojis to capture nuanced sentiments.
- **Negation Handling**: Special treatment of negation words to maintain sentence meanings.

## Phase 1: Baseline Modeling
- **Bag of Words (BoW)** and **TF-IDF** for initial frequency and importance analysis of words.
- **Word2Vec Embeddings**: To capture contextual meanings and associations, crucial for nuanced sentiment analysis.
- **Cosine Similarity**: Used to quantify similarities in tweet embeddings from Word2Vec, aiding in identifying sentiment clusters.

## Preliminary Results
- **WordCloud Visualizations**: Limited utility in sentiment insights from BoW and TF-IDF models, highlighting the need for context consideration.

## Phase 2: Advanced Modeling
- **Adjusted Preprocessing**: Use of a pre-trained Word2Vec model optimized with 50 dimensions for computational efficiency.
- **Supervised Machine Learning**: Utilization of Random Forest classifiers and exploration of N-grams for improved sentiment classification.
- **Performance Metrics**: Best F1 score achieved with N-grams at 0.73, indicating better contextual capture compared to other models.

## Sentiment Analysis
- **Contextual Analysis**: Use of sentence examples with positive/negative lexicons to refine model training and classification.
- **Performance Assessment**: Moderate performance with an F1 score around 0.53, suggesting further model refinement is needed.

## Conclusion
The project explored various sentiment analysis techniques with mixed effectiveness. The most successful approaches were found in adjusted preprocessing and N-grams usage in supervised machine learning, indicating avenues for further enhancement.

## Recommendations for Future Work
- **Deep Learning Models**: Exploration of LSTM and BERT for capturing deeper contextual nuances in text.
- **Real-Time Analysis**: Development of real-time sentiment analysis to process tweets as they are posted.
- **Sentiment Degree Identification**: Beyond binary classification to measure sentiment intensity.
- **Continuous Model Improvement**: Focused on enhancing model accuracy with additional lexicons and continuous learning.

## Installation and Usage
- **Dependencies**: Python 3.x, NLTK, Gensim, Scikit-Learn, Pandas, NumPy, Matplotlib
- **Setup**: Instructions on setting up the Python environment and installing dependencies.
- **Execution**: Step-by-step guide on how to run the analysis scripts.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
