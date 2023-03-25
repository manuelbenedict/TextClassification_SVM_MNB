# Mathematics Question Text Classification with Support Vector Machine (SVM) and Multinomial Naïve Bayes (MNB)

## About the Project
This is my Practical Work course research project as a research assistant for Mrs. Hasmawati, S.Kom., M.Kom., one of lecturer in Data Science at School of Computing, Telkom University. The research is about text classification implementation for Mathematics multiple choice questions in elementary and junior high schools with machine learning model, i.e. Support Vector Machine (SVM) and Multinomial Naïve Bayes (MNB). The question text is in Bahasa Indonesia. All questions will classify in three categories, i.e. easy, medium, and hard. </br></br>
Tools: Google Colab or Jupyter Notebook </br>
Programming language: Python </br>

## Dataset
The dataset is prepared by lecturer, which consist of Mathematics multiple choice questions for elementary and senior high schools. As a research assistant, one of my responsibilities is managed data with removing the duplicates data and invalid questions. Invalid questions contains the senteces or phrases which refer to tables and/or pitcure, e.g. "Perhatikan gambar berikut", "Perhatikan tabel berikut", "Dari gambar disamping", etc. Next, every data needs to be labelled. There are three labels for the question classification, i.e. easy, medium, and hard. There are a guide to label the dataset. The guide is in Bahasa Indonesia (Access the PDF with title "Labelling Guide").

## Preprocessing Data
The dataset needs to be prepared before it will be used into the models. For the Natural Language Processing (NLP) problem in general, there are some phases for preprocessing data, i.e. removing characters (punctuation, numbers, and symbols), removing stopwords, and stemming. Stemming text in Bahasa Indonesia is supported by Sastrawi library. After the preprocessing, the final is checking duplicates for once to keep the dataset variety.  

## Feature Extraction
The feature extraction purpose is to transform the text feature into numerical feature that can be processed. This project tries two feature extractions, i.e. Bag of Words (BoW) and TF-IDF (Term Frequency-Inverse Document Frequency). The BoW is the most basic feature extraction and earliest method, which the number feature is counted of each word (token) in a document. The TF-IDF is the feature extraction which is based on word occurrence frequency in the document. Both of feature extractions are supported by Scikit Learn library.

## Splitting Data
The dataset is splitted into training data and testing data with ratio 80:20 that means 80% of training data and 20% of testing data. Scikit learn library is also used for spiltting data.

## Machine Learning Models

### Support Vector Machine (SVM)
Support Vector Machine (SVM) is one of the regression methods or
classification of data based on previous data and modeling supervised first. SVM can conduct training and create a model that will be used for classification and prediction. SVM performs training by creating a line and forming a hyperplane and creating margins for each label by taking the vector (which will be referred to as the support vector) that is closest to the margins for the two labels. SVM has the advantage of grouping high-dimensional textual data. This algorithm includes the most superior machine learning algorithms in the classification. This is evidenced by the results of 5 previous studies using SVM for classification, especially text classification.

### Multinomial Naïve Bayes (MNB)
Multinomial Naïve Bayes (MNB) is the development of the Naïve Bayes model which produces a probability value of the frequency or number of words that appear in a sentence. This algorithm is a Naïve Bayes algorithm which is often used in text classification. This method, whose features are assumed from a simple multinomial distribution, has the main characteristic of being a strong (naïve) assumption of the independence between variables. This method also utilizes Bayes Theorem and data mining functionality, namely Naïve Bayesian Classification. MNB is able to consider the frequency of each word that appears in the document.

## Result
<table>
    <thead>
        <tr>
            <th>Layer 1</th>
            <th>Layer 2</th>
            <th>Layer 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=4>L1 Name</td>
            <td rowspan=2>L2 Name A</td>
            <td>L3 Name A</td>
        </tr>
        <tr>
            <td>L3 Name B</td>
        </tr>
        <tr>
            <td rowspan=2>L2 Name B</td>
            <td>L3 Name C</td>
        </tr>
        <tr>
            <td>L3 Name D</td>
        </tr>
    </tbody>
</table>
## Conclusion
