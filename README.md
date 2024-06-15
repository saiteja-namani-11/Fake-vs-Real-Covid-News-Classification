# Identifying Real vs. Fake COVID-19 News on Social Media: A Text Mining Approach

## Project Overview

This project aims to identify and classify content as genuine or fraudulent by applying text mining and machine learning approaches. By reducing the spread of false information, this research aids in combating the COVID-19 pandemic, supports public health authorities in distributing correct information, and helps social media platforms stop the spread of misinformation.

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [LDA Topic Modelling](#lda-topic-modelling)
6. [Methods](#methods)
7. [Ethical Considerations](#ethical-considerations)
8. [Conclusion](#conclusion)
9. [References](#references)

## Introduction

### Background

Social media is a vital information source for billions of people globally. By 2025, it is forecasted that the number of active users will rise to 4.41 billion. This surge highlights the importance of social media in the sharing and exchange of knowledge. Its ability to work quickly makes it possible to do a wide range of tasks, including improving brand awareness and speeding up consumer interaction and feedback channels.

### Significance of the Study

This study aims to create a solid foundation for identifying and classifying content as genuine or fraudulent using text mining and machine learning approaches. It hopes to reduce the spread of false information, aiding the global effort to combat the COVID-19 epidemic. This research is significant for public health authorities, social media platforms, and individuals, providing a standard for handling future emergencies in the digital sphere.

## Dataset Description

The dataset focuses on distinguishing between real and fake news related to the COVID-19 pandemic. It includes:

- **Real News Tweets:** Sourced from verified and credible sources, providing accurate information about COVID-19.
- **Fake News Tweets:** Contain claims or speculations about COVID-19 verified to be untrue, gathered from public fact-verification websites and social media platforms.

### Collection and Annotations

- Content is related to COVID-19.
- Only textual English content is considered.

## Data Preprocessing

Preprocessing steps included:
- Converting text to lowercase
- Removing URLs and user mentions
- Converting emojis to text
- Removing punctuation
- Tokenization

Stop words were not removed to maintain contextual understanding.

## Exploratory Data Analysis

### Word Cloud Visualizations

**Real Posts Word Cloud:**
- Prominent terms: "COVID-19," "case," "new," "people"
- Focus on reporting new cases and impacts on people, statistics, and data.

**Fake Posts Word Cloud:**
- Prominent terms: "covid19," "China," "Trump," "vaccine"
- Often include conspiracy theories or politically charged content.

## LDA Topic Modelling

LDA was used to systematically identify and categorize themes in large text datasets, helping to distinguish between false information and factual information.

### Analysis of Topics in Fake Tweets
- Fragmented themes, blending accurate details with irrelevant or deceptive information.

### Analysis of Topics in Real Tweets
- Cohesive and contextually relevant themes, focusing on geographical allusions, healthcare data, and COVID-19 statistics.

## Methods

### Models Used

- **Support Vector Machine (SVM)**
- **XGBoost**
- **AdaBoost**
- **BERT**
- **BERT + BiLSTM**

Each model was evaluated based on accuracy, precision, recall, and F1 score.

### Performance Overview

**Support Vector Machine (SVM):**
- Accuracy: 92.68%
- F1 Score: 93.06%

**XGBoost:**
- Accuracy: 91.12%
- F1 Score: 91.40%

**AdaBoost:**
- Accuracy: 84.27%
- F1 Score: 84.77%

**BERT:**
- Accuracy: 95.48%
- F1 Score: 95.84%

**BERT + BiLSTM:**
- Accuracy: 97.89%
- F1 Score: 97.92%

## Ethical Considerations

The project adhered to ethical standards, ensuring:
- Accuracy and non-bias in analysis
- Mitigation of harm by responsible communication
- Ethical use of data, maintaining privacy and confidentiality

## Conclusion

### Model Accuracy Table

| Model       | Accuracy | F1-Score | Precision | Recall |
|-------------|----------|----------|-----------|--------|
| SVM         | 91.40    | 91.80    | 91.71     | 91.87  |
| XGBoost     | 88.60    | 88.97    | 90.03     | 87.95  |
| AdaBoost    | 83.73    | 84.12    | 86.00     | 82.32  |
| BERT        | 96.10    | 96.33    | 97.62     | 95.08  |
| BERT+BILSTM | 93.92    | 94.42    | 93.48     | 95.37  |

BERT and BERT + BiLSTM stand out as the most effective models for classifying COVID-19 related tweets, excelling in contextual understanding and processing sequential information.

## References

1. [NCBI Article 1](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8608495/)
2. [IEEE Explore Document](https://ieeexplore.ieee.org/document/9803414)
3. [NCBI Article 2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10197436/)
4. [Arxiv Paper](https://arxiv.org/ftp/arxiv/papers/2203/2203.09936.pdf)
5. [ChatGPT](https://chat.openai.com/)
