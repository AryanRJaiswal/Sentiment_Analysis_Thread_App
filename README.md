# Sentiment Analysis on Thread App
- This repository contains a Python script for performing sentiment analysis on a dataset of app reviews. The script reads a CSV file of reviews, processes the text to calculate sentiment scores using TextBlob, and categorizes the reviews into positive, negative, or neutral ratings.

### Dataset
- The dataset used in this project contains 36,943 rows and 14 columns, which include user reviews and metadata such as the review description, rating, and additional developer responses. For simplicity, unnecessary columns are dropped before analysis.
Upload the Dataset: The script uses Google Colab's file upload functionality to upload the dataset. You need to upload the dataset in CSV format. In this case, the dataset 37000_reviews_of_thread_app.csv.zip is used.

### Data Preprocessing:

- Duplicate rows are checked and removed.
- Unnecessary columns such as review_title, developer_response, and appVersion are dropped to focus on the relevant text data.

### Sentiment Analysis:

- The sentiment of each review description is analyzed using TextBlob's polarity scoring function. A custom function is used to classify each score into Positive, Negative, or Neutral categories.

### Rating Analysis:

- Reviews are also classified based on their star ratings. Ratings of 4 or higher are considered positive, ratings of 2 or below are negative, and ratings of 3 are neutral.

### Final Rating:

- A final rating is determined by comparing both the text sentiment and the star rating. The combination results in a Positive, Negative, or Neutral classification.

### Visualization:

- The script uses Seaborn's countplot to visualize the distribution of the final ratings.
