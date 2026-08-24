# Email Spam Classification System

A machine learning project that classifies email messages as **Spam** or **Ham (legitimate)** using natural language processing and supervised machine learning.

## Project Overview

Spam emails are unwanted messages that may contain advertisements, misleading information, or potentially harmful content. This project explores how machine learning can be used to automatically classify email messages based on patterns learned from previously labelled data.

The project compares multiple classification algorithms and evaluates their performance on unseen test data.

## Dataset

The project uses a labelled dataset containing **5,171 email messages**:

- 3,672 Ham emails
- 1,499 Spam emails

Each record contains the email text and its corresponding Spam/Ham label.

## Methodology

The project follows these steps:

1. Load and inspect the dataset
2. Handle missing values
3. Encode labels:
   - Spam → 0
   - Ham → 1
4. Split the data into training and testing sets using an 80:20 stratified split
5. Convert email text into numerical features using **TF-IDF**
6. Train multiple machine learning classification models
7. Evaluate the models using test-set accuracy and confusion matrices
8. Compare model performance
9. Use the trained model to classify new email text

## Machine Learning Models

The following models were implemented and compared:

- Logistic Regression
- Naive Bayes
- Decision Tree
- Random Forest

Logistic Regression was trained using balanced class weights to account for the difference between the number of Spam and Ham examples.

## Results

| Model | Test Accuracy |

| Logistic Regression | 97.10% |
| Naive Bayes | 90.24% |
| Decision Tree | 90.43% |
| **Random Forest** | **98.16%** |

Random Forest achieved the highest test accuracy among the evaluated models.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab
- TF-IDF

