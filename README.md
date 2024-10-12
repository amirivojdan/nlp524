# Natural Language Processing - COSC 524

## Project 1 - Authorship Atrribution

This project tackles the classic problem of authorship attribution in computational linguistics and stylometry. The code implements a binary classification system to determine whether a given text was written by a specific target author or by other crime novelists.
The solution begins with dataset preparation, where novels from Project Gutenberg are collected and preprocessed. The preprocessing steps include cleaning the text by removing Project Gutenberg headers and footers, and then splitting the novels into smaller chunks to improve training results. This chunking approach is particularly useful for handling long texts, as seen in the code where each novel is divided into sentence chunks of a specified size.
For feature engineering, the project employs both Bag of Words (BoW) and Term Frequency-Inverse Document Frequency (TF-IDF) representations. These are standard techniques in NLP for converting text into numerical features suitable for machine learning models. The code also extracts basic stylometric features such as word lengths and sentence lengths, which can capture aspects of an author's writing style.
The model development phase explores several classical machine learning algorithms as suggested in the project description. The code implements a Ridge Classifier, Support Vector Machine (SVM), and Random Forest Classifier. These models are trained on both BoW and TF-IDF features, allowing for a comparison of their effectiveness in this authorship attribution task.
