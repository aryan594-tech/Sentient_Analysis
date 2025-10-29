# Sentient_Analysis
Demonstrates a comprehensive sentiment analysis implementation using natural language processing and deep learning techniques. The project analyzes text data to classify sentiments into categories such as positive, negative, or neutral.
# Sentiment Analysis Project

This project performs sentiment analysis on customer reviews from the "Reviews.csv" dataset. The goal is to analyze the sentiment expressed in the reviews and compare the results obtained from different sentiment analysis methods.

## Methods Used

The project utilizes two sentiment analysis methods:

1.  **VADER (Valence Aware Dictionary and sEntiment Reasoner):** A lexicon and rule-based sentiment analysis tool specifically attuned to sentiments expressed in social media.
2.  **Roberta Pretrained Model:** A transformer-based model trained on a large corpus, which considers the context of words for more nuanced sentiment analysis.

## How to Run the Notebook

This project is implemented as a Google Colab notebook. To run the analysis:

1.  Ensure you have access to the "sentiment analysis" GitHub repository.
2.  Open the Colab notebook file (e.g., `sentiment_analysis.ipynb`) in Google Colab.
3.  Make sure the `Reviews.csv` dataset is available in the Colab environment (e.g., uploaded or cloned with the repository).
4.  Install the necessary libraries by running the first code cell:
    ```bash
    !pip install pandas numpy matplotlib seaborn nltk transformers scipy
    ```
5.  Run the remaining cells in the notebook sequentially.

## Notebook Steps

The notebook performs the following key steps:

1.  **Data Loading and Exploration:** Loads the `Reviews.csv` dataset and performs a quick exploratory data analysis (EDA) to understand the distribution of review scores.
2.  **VADER Sentiment Analysis:** Applies the VADER sentiment intensity analyzer to each review text to obtain negative, neutral, positive, and compound sentiment scores.
3.  **Roberta Sentiment Analysis:** Utilizes a pretrained Roberta model from the `transformers` library to calculate negative, neutral, and positive sentiment scores for each review text.
4.  **Comparison of Results:** Merges the sentiment scores from both VADER and Roberta with the original DataFrame and visualizes the correlation between the scores and the review stars.
5.  **Review Examples:** Examines examples of reviews where the model scores and the actual star ratings might differ.

## Key Findings (Optional)

[Include any interesting observations or comparisons between VADER and Roberta results here after running the notebook. For example, you could mention if one model seems to align better with the star ratings or if they capture different aspects of sentiment.]
