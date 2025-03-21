# Cutomer-review-analysis-NLP

## Problem Statement

ShopEase receives thousands of customer reviews daily. Manually going through these reviews to identify major themes such as product quality, delivery issues, pricing, and customer support is time-consuming and inefficient.

## Goal

Automate the process of discovering key topics in customer feedback. This will help ShopEase’s customer service and product teams quickly address concerns and improve overall customer satisfaction. Additionally, analyze the sentiments of the customers to determine if they are positive, negative, or neutral.

### Approach

### 1. Data Exploration and Preprocessing

1. Loaded the dataset and examined the first few rows to understand the data structure.

2. Checked for missing values to handle data inconsistencies.

3. The dataset contained columns: review_text, rating, category, and timestamp.

4. Performed basic EDA (Exploratory Data Analysis) and visualizations to analyze the distribution of ratings and product categories.

### 2. Data Cleaning

1. Converted text to lowercase.

2. Removed alphanumeric characters and special symbols.

3. Removed stopwords.

4. Tokenized the text for further processing.

### 3. Exploratory Data Analysis (EDA)

1. Used WordCloud to visualize the most frequently occurring words in the dataset.

2. Extracted 20 most common words using nltk.FreqDist().most_common() and represented them in a bar chart for better understanding.

### 4. Topic Modeling (LDA - Latent Dirichlet Allocation)

1. Created a dictionary and corpus from the cleaned text data.

2. Applied LDA (Latent Dirichlet Allocation) with passes=5, categorizing customer reviews into 5 main topics.

3. Generated WordClouds for each topic to interpret the topic distribution visually.

4. Uploaded a separate test file containing sentences to verify the model’s accuracy in topic classification.

### 5. Sentiment Analysis

1. Used VADER (Valence Aware Dictionary and sEntiment Reasoner) to analyze the sentiment of customer reviews.

2. Represented sentiment distribution using visualizations based on:

Topics

Ratings

Overall sentiment (Positive, Negative, Neutral)

### 6. Model Evaluation

Calculated Coherence Score using Gensim to evaluate the topic model’s performance.

### Results

1. Identified key themes in customer feedback.

2. Provided sentiment insights to understand customer satisfaction levels.

3. Enabled the customer service and product teams to make data-driven decisions for improving user experience.
