# Sentiment Analysis on Twitter Data Regarding the Aarogya Setu App

## Abstract

This project focuses on studying the impact of the alleged hacking of the "Aarogya Setu" app on people's opinions and sentiments. The app, launched by the Government of India to track COVID-19 cases, became the subject of controversy after claims of a security breach. This research analyzes Twitter data to determine how the public sentiment towards the app evolved before and after the hacking allegations.

The complete paper detailing the methodology and findings of this research can be found here [IEEE Explore](https://ieeexplore.ieee.org/abstract/document/9299634).

## Keywords
- Aarogya Setu
- Sentimental Analysis
- Opinion Mining
- COVID-19
- Twitter Data
- Digital India
- Qualitative Research

## 1. Introduction

Aarogya Setu is a contact tracing app launched by the Government of India in April 2020 to help track COVID-19 spread. Despite its rapid adoption, the app faced allegations of hacking, leading to concerns about user privacy and security. This project aims to assess how these allegations affected public sentiment towards the app by analyzing Twitter data. 

## 2. Literature Review

Sentiment analysis and opinion mining have emerged as crucial tools for understanding public emotions, especially on platforms like Twitter, where users openly express their opinions. Previous studies have used sentiment analysis for various domains, including tracking public sentiment about health-related apps, social issues, and more.

## 3. Research Methodology

This study employs a qualitative research approach. The sentiment of Twitter users before and after the alleged hacking of the app was compared by extracting relevant tweets. Since Twitter’s official API had restrictions on accessing older tweets, we used the **GetOldTweets3** library to collect tweets. After data collection, text preprocessing techniques such as tokenization, stemming, and removal of stop words were applied. Sentiment analysis was performed using the **Afinn** library to classify tweets as positive, negative, or neutral.

## 4. Data Collection

- **Post-Alleged Hacking Data**: Collected from May 5 to May 20, 2020, resulting in 3,550 tweets.
- **Pre-Alleged Hacking Data**: Collected from April 2 to April 17, 2020, resulting in 5,002 tweets.

Tweets were filtered by the hashtag "#AarogyaSetu" and only English-language tweets were considered.

## 5. Data Pre-processing

The following steps were carried out on the raw data:

- **Stemming**: Removed suffixes like "-ing", "-tion", etc.
- **Tokenization**: Removed emoticons, expanded acronyms, and fixed spelling mistakes.
- **Stop Words Removal**: Removed common words with no relevance to the sentiment (e.g., "a", "an", "the", etc.).

## 6. Sentiment Analysis & Polarity Classification

The collected and preprocessed data was analyzed using sentiment analysis tools. The sentiment was categorized into three classes: positive, negative, and neutral. The sentiment of tweets was computed using the **Afinn** sentiment score.

### Libraries Used:
- **Numpy, Pandas**: Data manipulation and analysis.
- **Matplotlib**: Data visualization (pie charts, word clouds).
- **NLTK**: Text preprocessing and sentiment analysis.
- **GetOldTweets3**: Collecting historical Twitter data.

## 7. Results

The sentiment analysis results indicate a significant rise in negative sentiments regarding the Aarogya Setu app after the alleged hacking news. The frequency of negative tweets increased, while the positive sentiment declined.

### Word Frequency (Before and After Alleged Hacking):

| **Top Words Before Alleged Hacking** | **Frequency** |
|--------------------------------------|---------------|
| aarogyasetu                          | 4102          |
| app                                  | 2709          |
| covid19                              | 1503          |
| download                             | 1140          |
| narendramodi                         | 1053          |

### Sentiment Distribution (Pie Charts):

- **Pre-Hacking Sentiments**: A majority of tweets were neutral or positive.
- **Post-Hacking Sentiments**: A significant shift towards negative sentiments.

## 8. Conclusion

The study concludes that the alleged hacking of the Aarogya Setu app had a noticeable negative impact on public sentiment. This was reflected in the increased volume of negative tweets and the overall sentiment shift on social media.


## 🌍 Explore More Projects  
For more exciting machine learning and AI projects, visit **[The iVision](https://theivision.wordpress.com/)** and stay updated with the latest innovations and research! 🚀  

---
