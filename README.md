# Telegram App Review Analytics

Comprehensive NLP analysis of 100,000 Telegram app user reviews for sentiment classification and topic extraction.

## Overview

This project analyzes 100,000 Telegram app reviews to:
- Classify sentiment (Negative, Neutral, Positive) with 85% accuracy
- Extract key topics using BERTopic modeling
- Deliver actionable insights for product development

## Interactive Application

A Streamlit web application is available for real-time sentiment prediction and visualization. Users can input Telegram app reviews and receive instant sentiment classification with confidence scores.

**Try the app:** [Click Here](https://telegram-sentiment-app-qmrbibgrmyeufurewm9whs.streamlit.app/)

## Key Findings

- 60.1% of reviews express negative sentiment
- 42.7% of complaints relate to authentication and OTP failures
- 62.4% of positive feedback highlights Premium features
- Review volume surged 83% YoY in early 2025, then dropped 44% by year-end

## Methodology

**Sentiment Classification**
- TF-IDF feature extraction with n-grams
- Logistic Regression selected from 10+ algorithms
- Hyperparameter optimization using Optuna
- Threshold calibration for improved minority class detection

**Topic Modeling**
- BERTopic with multilingual-MiniLM-L12-v2 embeddings
- HDBSCAN clustering for semantic grouping
- c-TF-IDF for keyword extraction
- Coherence Score validation for optimal topic count

## Model Performance

- F1-Score (Macro): 0.66
- Accuracy: 85%
- Recall (Negative): 96%
- Recall (Positive): 79%
- Topic Coverage: 97.9% (Negative), 95.2% (Positive)

## Tech Stack

- Natural Language Processing: BERTopic, TF-IDF, multilingual-MiniLM-L12-v2
- Machine Learning: Logistic Regression, HDBSCAN
- Optimization: Optuna (Bayesian optimization)
- Analysis: Coherence Score, Stratified Cross-Validation
- Deployment: Streamlit

## Strategic Recommendations

**Authentication Issues (42.7% of negative reviews)**
- Audit SMS gateway providers in high-failure regions
- Implement alternative login methods (WhatsApp, Email verification)

**Monetization Concerns (2.6x increase in Q4 2025)**
- Investigate pricing changes and bugs in October-December releases
- Fix premium login loops preventing paid user access

**Product Strengths**
- Leverage high satisfaction with Premium features (91% satisfaction rate)
- Prioritize file sharing and group functionality in marketing
- Focus on business user segment with highest retention

## Repository Contents

For complete analysis details, methodology, and visualizations, refer to the PDF documentation included in this repository.

## Author

Az-Zukhrufu Fi Silmi Suwondo

- Email: afsilmis@gmail.com
- LinkedIn: [az-zukhrufu-fi-silmi-suwondo](https://linkedin.com/in/az-zukhrufu-fi-silmi-suwondo/)
- GitHub: [@afsilmis](https://github.com/afsilmis/)

## Data Source

Dataset: [Kaggle/pandaa12](https://www.kaggle.com/datasets/pandaa12/telegram-reviews-indonesia-google-play-store)
