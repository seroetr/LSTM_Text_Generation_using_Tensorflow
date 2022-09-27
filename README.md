## Text Generation
- LSTM Text Generation using Tensorflow
## Multi-Label Text Classification
- `stackoverflow.csv` dataset is used, which can be found via link: https://raw.githubusercontent.com/laxmimerit/All-CSV-ML-Data-Files-Download/master/stackoverflow.csv
- `Tf-idf` and `MultiLabelBinarizer` are used together to prepare train and test dataset from csv file.
- Since Logistic Regression and SVM don't support multi-class classification, OneVsRestClassifier is used.
- The One-vs-Rest strategy splits a multi-class classification into one binary classification problem per class.
## Hate Speech Classification
- In Tensorflow, Convolutional Neural Network is used to perform hate speech classification.
- Dataset file is `adele.txt` can be reached via https://raw.githubusercontent.com/laxmimerit/hate_speech_dataset/master/data.csv.
- First data preprocessing is realized. After that, since the dataset is not huge, only one layer CNN model is built.
- Using `from tensorflow.keras.preprocessing.text import Tokenizer`, numerical values are assigned to words in dictionary format so that each word has its own word_index.
- Each sentence will be converted into a sequence where each word is replaced by its number in the word index using `tokenizer.texts_to_sequences(sentences)`.
