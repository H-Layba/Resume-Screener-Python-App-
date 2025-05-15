# Resume-Screener-Python-App-
A machine learning-powered web app that automatically classifies resumes into job categories such as Data Science, Java Developer, DevOps Engineer, and more.

<!-- Optional screenshot -->

# Overview
The Resume Screener project leverages Natural Language Processing (NLP) and machine learning to analyze resumes and predict the most relevant job category. Built using Python, scikit-learn, and Streamlit, this tool is useful for HR professionals and recruiters to streamline the resume screening process.

# Features
Clean and preprocess resume text using NLP techniques.

Train a classifier (K-Nearest Neighbors with One-vs-Rest strategy).

Transform resume data using TF-IDF vectorization.

Predict job category from uploaded resumes.

Streamlit web interface for easy resume upload and classification.

# Project Structure
Resume Screener:

- app.py                     
- ResumeScreener.ipynb       
- tfidf.pkl                  
- UpdatedResumeData.csv      
- README.md       


# Categories Predicted
Data Science

Python Developer

Java Developer

Web Designing

DevOps Engineer

HR

Blockchain

Business Analyst

Testing

Sales

and many more...

(Full list in app.py's category_mapping)

# Model & Data
Dataset: UpdatedResumeData.csv containing resumes and labeled job categories.

Text Processing: Custom cleaning + TF-IDF vectorization.

Classifier: KNeighborsClassifier wrapped with OneVsRestClassifier.

# How to Run
Prerequisites
Python 3.7+

# Install required libraries:

pip install -r requirements.txt

Or manually install:

pip install streamlit scikit-learn pandas numpy nltk matplotlib seaborn

# Launch the App

streamlit run app.py

# Upload Formats Supported
.txt
.pdf (Note: PDF parsing is done via UTF-8 or Latin-1 decoding. Some formats may not be fully supported.)

# Model Training:
To retrain or improve the model, refer to ResumeScreener.ipynb, which includes:

EDA (Exploratory Data Analysis)

Cleaning and preprocessing

Label encoding

TF-IDF vectorization

Model training and evaluation

Pickling the trained model and vectorizer

# Testing the App:
You can test the system by copying a resume snippet into myresume variable in the notebook or uploading it via the Streamlit interface.
