# Multiclass Text Classification SatriaData2024
This project was created as a requirement for the preliminary round of Satria Data 2024.
# Description
In this project, analysis and model development for multi-class text classification were conducted. The data used consisted of text data related to elections (Pemilu). Several experimental scenarios were carried out to identify the best model, and it was found that the best model is the BERT model.
# Data
The data used was provided by the organizers. It consists of training and test data, containing two attributes/columns: the text column and its label. The data is classified into 8 classes: Demografi, Ekonomi, Geografi, Ideologi, Perhanan dan Keamanan, Politik, Sosial Budaya, and Sumber Daya Alam. According to the competition description, there is challenges in the data include issues like misspellings or typos, ambiguity, and non-standard words
# Pre-processing
Several preprocessing steps were carried out, such as cleaning the data using regex, creating a dictionary to convert abbreviated words, using the IndoNLP library to normalize slang and elongated words, removing stopwords, and performing stemming.
# Model
Various models were tested to find the one with the best performance. The models tested include LSTM, GRU, and BERT. Experiments were conducted by tweaking their hyperparameters. The evaluation metric used was balanced accuracy due to the imbalanced data. It was found that the BERT model had the best performance. The BERT model used was the pre-trained **indobenchmark/indobert-base-p1** model, which was fine-tuned using the training data. As a result, this model achieved a score of 0.70 on the test data.
