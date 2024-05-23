# Analyzing Customer Support Tweets: Understanding Sentiments and Trends


## Overview
The proliferation of social media platforms has transformed the way companies interact with their customers. X (Twitter), in particular, has become a prominent channel for customer support, allowing companies to engage with customers in real time. This project focuses on analyzing customer support tweets to gain insights into customer sentiments and identify trends over time.

## Table of Contents
- [Introduction](##introduction)
- [Data Collection and Preprocessing](#Data-Collection-and-Preprocessing)
- [Sentiment Analysis](#SentimentAnalysis)
- [Trend Analysis](#Trend-Analysis)
- [Holiday Analysis](#Holiday-Analysis)
- [Additional Analysis](#Additional-Analysis)
- [Conclusion](#Conclusion)
- [ Insights and Recommendations](#Insights-and-Recommendations)
- [Future Work](#FutureWork)
- [References](#References)
- [How to Run the Code](#how-to-run-the-code)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Authors](#authors)
- [Acknowledgments](#acknowledgments)

## Introduction
Social media platforms like Twitter have become crucial for customer service and support. Companies engage with customers through these channels to resolve issues and gather feedback. This project analyzes customer support tweets to understand sentiments and identify trends over time.

## Project Objectives
1. Sentiment Analysis: Classify customer support tweets into positive, neutral, or negative categories to understand the overall sentiment of customer interactions.
2. Trend Identification: Examine tweet volumes and sentiments to identify patterns and trends, including seasonal variations and peak periods.
3. Issue Analysis: Investigate common customer issues during specific times, such as holidays, to better understand customer needs and challenges.

## Importance

1. Enhancing Customer Experience: By analyzing sentiments and trends, companies can better understand customer satisfaction and pinpoint areas for improvement.
2. Proactive Customer Support: Identifying recurring issues allows companies to address them proactively, improving overall service quality.
3. Efficient Resource Allocation: Understanding peak periods for customer support interactions helps in optimizing resource allocation to manage workloads effectively.
4. Strategic Decision Making: Insights from tweet analysis can inform strategic decisions to enhance customer support operations and customer relationship management.

## Data Collection and Preprocessing
### Description of the Dataset

The dataset consists of customer support tweets collected from Twitter. Each tweet includes information such as the text of the tweet, the date and time it was created, and other metadata.

### Preprocessing Steps

1. Loading the Dataset:

python code snippet
import pandas as pd
filtered_data = pd.read_csv('customer_support_tweets.csv')

2. Removal of stopwords
3. Stemming
4. Converting Dates:
python code snippet
filtered_data['created_at'] = pd.to_datetime(filtered_data['created_at'], errors='coerce')
5. Handling Missing Values:


6. Filter the data to focus on customer feedback
7. Feature Extraction:


## Sentiment Analysis
### Methodology

Sentiment analysis was performed using the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool. Each tweet was assigned a sentiment score indicating whether it was positive, negative, or neutral.

Distribution of Sentiment Scores

sentiment_counts = filtered_data['sentiment_category'].value_counts()
sns.barplot(x=sentiment_counts.index, y=sentiment_counts.values)
plt.title('Sentiment Distribution of Customer Support Tweets')
plt.xlabel('Sentiment')
plt.ylabel('Number of Tweets')
plt.show()

Examples of Tweets

positive    20015
neutral      7221
negative     6201
Positive: "Thank you for the quick response and resolution!"
Neutral: "I have a question about my account."
Negative: "I am very disappointed with the service I received."

## Trend Analysis
Identifying Trends and Patterns
The results section will contain visual representations of the discovered topics and their frequencies, along with an analysis of these findings.

Visualization of Tweet Volume Over Time

## Holiday Analysis
Tweet Interactions During Holidays
Based on the prevalent topics discovered from the customer reviews, we provide actionable insights and recommendations for product improvements and marketing strategies.

Analysis of Issues During Holidays

## Additional Analysis
### Word Cloud Visualization

## Conclusion
## Summary of Findings

### Sentiment Analysis: Majority of tweets were neutral, with a significant portion being positive. However pre 2014 majority of tweets were negative
### Trend Analysis: Identified peak periods and seasonal variations in tweet volumes and sentiments.
### Holiday Analysis: Increased interactions during holidays with varied sentiments indicating specific customer issues.

## Insights and Recommendations
- Improve Customer Support: Focus on addressing common issues highlighted in negative tweets.
- Resource Allocation: Allocate more resources during identified peak periods and holidays.

## Future Work
### Suggestions for Further Analysis

- Enhanced Sentiment Analysis: Incorporate more sophisticated NLP techniques for better sentiment classification.
- Customer Segmentation: Analyze tweets based on customer demographics to provide personalized support.
- Real-Time Analysis: Develop real-time monitoring tools for customer support interactions.

### Potential Areas for Research

- Impact of Support Quality on Customer Retention: Study the long-term impact of support quality on customer loyalty.
- Comparison Across Platforms: Compare customer support interactions across different social media platforms.

## References
[Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
[Seaborn Documentation](https://seaborn.pydata.org/)
[VADER Sentiment Analysis](https://github.com/cjhutto/vaderSentiment)
[WordCloud Documentation](https://github.com/amueller/word_cloud)

### Code Snippets

- Data Preprocessing Code
- Sentiment Analysis Code
- Visualization Code

## How to Run the Code
1. Clone the repository.
2. Install the required dependencies.
3. Run the `select_file()` function to load and process the dataset.
4. View the generated visualizations and analyze the extracted topics.

## Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/VincentLangat033/customer_support_data_analysis.git
    cd customer_support_data_analysis
    ```
2. Install the necessary packages:
    ```bash
    pip install -r requirements.txt
    ```
<!--
## Usage
--1. Run the script:
    ```bash
    python .py
    ```
2. Select the dataset file when prompted.
3. The script will preprocess the data, perform topic modeling, and display visualizations of the discovered topics.
-->
<!-- wewew
wewr -->
## Contributing
We welcome contributions to this project. Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Authors
- Vincent Langat
- Chrispus Kyalo
- Denis Kaniu
- Ken Makudha


