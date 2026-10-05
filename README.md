# Project 4 - NLP & Sentiment Analysis

## Overview

This project focuses on Natural Language Processing (NLP) and Sentiment Analysis. The goal is to process unstructured movie reviews, convert text into numerical features using TF-IDF, and train a machine learning model to classify reviews as Positive or Negative.

The project was completed as part of the Data Science Internship at DecodeLabs.

## Objective

The main objective of this project is to build an NLP-based sentiment classification system that can understand text reviews and predict their sentiment.

The project includes:

* Text preprocessing
* Tokenization
* Stop-word removal
* Lemmatization
* TF-IDF text vectorization
* Machine learning classification
* Model evaluation
* Prediction of sentiment for new reviews

## Dataset

The project uses the **IMDB Movie Reviews Dataset**, containing 50,000 movie reviews with two sentiment classes:

* Positive
* Negative

The dataset contains the following main columns:

* `review` - The movie review text
* `sentiment` - The sentiment label

## Technologies and Libraries

* Python
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## Project Workflow

### 1. Data Loading

The IMDB dataset was loaded using Pandas and inspected to understand its structure and contents.

### 2. Text Preprocessing

The reviews were cleaned and prepared for machine learning.

The preprocessing pipeline included:

* Converting text to lowercase
* Removing HTML tags
* Removing punctuation and special characters
* Tokenization
* Stop-word removal
* Lemmatization

### 3. Train-Test Split

The dataset was divided into:

* 80% training data
* 20% testing data

This resulted in:

* 40,000 training reviews
* 10,000 testing reviews

### 4. TF-IDF Vectorization

TF-IDF (Term Frequency-Inverse Document Frequency) was used to convert the cleaned text into numerical features that could be processed by a machine learning algorithm.

The final TF-IDF representation used 10,000 features.

### 5. Machine Learning Model

A **Linear Support Vector Machine (SVM)** classifier was trained using the TF-IDF features.

The trained model was then used to predict the sentiment of unseen movie reviews.

### 6. Model Evaluation

The model was evaluated using accuracy and a classification report containing precision, recall, and F1-score.

The achieved accuracy was:

**89.13%**

A confusion matrix was also generated to visualize the model's predictions.

### 7. New Review Prediction

The project also includes a prediction function that accepts a new movie review, applies the same preprocessing and TF-IDF transformation, and predicts whether the review is Positive or Negative.

## Project Structure

```text
NLP_Sentiment_Project/
│
├── sentiment_analysis.ipynb
├── IMDB Dataset.csv
├── README.md
└── requirements.txt
```

## How to Run

1. Clone or download the project.
2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Open `sentiment_analysis.ipynb` in VS Code or Jupyter Notebook.
4. Make sure the IMDB dataset CSV is available in the project folder.
5. Run the notebook cells from beginning to end.

## Results

| Metric           |     Result |
| ---------------- | ---------: |
| Total Reviews    |     50,000 |
| Training Reviews |     40,000 |
| Testing Reviews  |     10,000 |
| TF-IDF Features  |     10,000 |
| Model            | Linear SVM |
| Accuracy         |     89.13% |

## Key Skills Demonstrated

* Natural Language Processing
* Text preprocessing
* Tokenization
* Stop-word removal
* Lemmatization
* TF-IDF vectorization
* Machine learning classification
* Model evaluation
* Unstructured data handling

## Conclusion

This project demonstrates how unstructured human language can be transformed into numerical data and processed using machine learning. The Linear SVM classifier achieved an accuracy of 89.13% on the test dataset, successfully classifying movie reviews into Positive and Negative sentiment categories.
