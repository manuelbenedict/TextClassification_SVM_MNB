# Mathematics Question Text Classification with Support Vector Machine (SVM) and Multinomial Naïve Bayes (MNB)

## About the Project
This is my Practical Work course research project as a research assistant for Mrs. Hasmawati, S.Kom., M.Kom., one of lecturer in Data Science at School of Computing, Telkom University. The research is about text classification implementation for Mathematics multiple choice questions in elementary, junior high, and senior high schools with machine learning model, i.e. Support Vector Machine (SVM) and Multinomial Naïve Bayes (MNB). The question text is in Bahasa Indonesia. All questions will classify in three categories, i.e. easy, medium, and hard. </br></br>
Tools: Google Colab or Jupyter Notebook </br>
Programming language: Python </br>

## Dataset
The dataset is prepared by lecturer, which consist of Mathematics multiple choice questions for elementary, junior high, and senior high schools. As a research assistant, one of my responsibilities is managed data with removing the duplicates data and invalid questions. Invalid questions contains the senteces or phrases which refer to tables and/or pitcure, e.g. "Perhatikan gambar berikut", "Perhatikan tabel berikut", "Dari gambar disamping", etc. Next, every data needs to be labelled. There are three labels for the question classification, i.e. easy, medium, and hard. There are a guide to label the dataset. </br></br>
The guide is in Bahasa Indonesia (Access the PDF with title "Labelling Guide").

## Preprocessing Data
The dataset needs to be prepared before it will be used into the models. For the Natural Language Processing (NLP) problem in general, there are some phases for preprocessing data, i.e. removing characters (punctuation, numbers, and symbols), removing stopwords, and stemming. Stemming text in Bahasa Indonesia is supported by Sastrawi library in Python. After the preprocessing, the final is checking duplicates for once to keep the dataset variety.  

## Feature Extraction
The feature extraction purpose is to transform the text feature into numerical feature that can be processed. This project tries two feature extractions, i.e. Bag of Words (BoW) and TF-IDF (Term Frequency-Inverse Document Frequency). The BoW is the most basic feature extraction and earliest method, which the number feature is counted of each word (token) in a document. The TF-IDF is the feature extraction which is based on word occurrence frequency in the document. Both of feature extractions are supported by Scikit Learn library in Python.

## Splitting Data


## Machine Learning Models


## Conclusion
