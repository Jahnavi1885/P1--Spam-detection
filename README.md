# email-spam-classifier-new

End to end code for the email spam classifier project
This project is an AI-based system that classifies emails as either “Spam” or “Not Spam” (Ham) using Natural Language Processing (NLP) and Machine Learning algorithms. It automatically filters out unwanted messages like ads, phishing attempts, and promotions, while keeping important emails safe.

How It Works

Dataset Collection
Uses labeled datasets containing examples of spam and non-spam emails.
Example: Enron dataset, SMS Spam Collection dataset.
Data Preprocessing (NLP)
Convert raw email text into a clean format:
Lowercasing text
Removing stopwords, punctuation, and special characters
Stemming/Lemmatization to reduce words to base forms
Feature Extraction
Convert text into numerical features using:
Bag of Words (BoW) or
TF-IDF (Term Frequency–Inverse Document Frequency)
Each email is represented as a vector of word frequencies.

Model Training
Machine learning algorithms are trained on these features, such as:
Naive Bayes (commonly used and very effective)
Support Vector Machines (SVM)
Random Forest / Logistic Regression
The model learns to distinguish spam patterns (e.g., “win money”, “lottery”, “free offer”).
Prediction
When a new email comes in, the system preprocesses it, extracts features, and passes it through the trained model.
Output: Spam or Not Spam.
Evaluation
Accuracy, Precision, Recall, and F1-Score are used to measure performance.
A confusion matrix shows how well the system identifies spam vs. non-spam.

Tech Stack
Python
NLP Libraries: NLTK, SpaCy
ML Libraries: Scikit-learn, Pandas, NumPy
Algorithms: Naive Bayes (most common for spam detection), SVM, Logistic Regression
