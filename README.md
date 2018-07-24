# Spam_Classification using (RNN-LSTM)

## Required Packages
1. Pandas
2. Numpy
3. Codecs
4. NLTK
5. Tensorflow

### Dataset Enron1 was downloaded from (http://nlp.cs.aueb.gr/software_and_datasets/Enron-Spam/preprocessed/enron1.tar.gz) for this RNN-LSTM Email Spam Classifier.

## Dataset Preparation

### I did a the following prepossessing on the Dataset:

1. Applied Regex for replacing website, clocktime, date, alphanumeric, digits.
2. Converting Unicode to Ascii.
3. Removing punctuation from sentences.

## Feature Representation Techniques
 1. Made a Dictionary of vocabulary and their count
 2. Converted sentences in the form of their vocabulary counts
 3. Making each sentences of the length 3559 by left padding with zeros, as maximum length of the sentences was 3559.
 4. Making labels into binary 0 and 1
 5. Shuffling Our Dataset
 6. Splitting Dataset into Train, Test and Validation Sets (80% of data is kept in the training set and of the remaining data 50% in the validation set and 50% in training set.)

## Model Building

1. Assigning the Hyperparameters For RNN_LSTM.
2. Create the graph object
3. Add nodes to the graph
4. Converting Words to Word Embeddings
5. Defining our LSTM cell
6. Defining our Loss Function and Optimization Function
7. Setting up our Evaluation and Accuracy matrics
8. Batching
9. Training the RNN_LSTM Model
10. Testing the RNN_LSTM Model

### I trained the model for only 2 epochs with a batch size of 50 (as I have an Intel Core i5 7th gen with 8gb RAM which was having thermal trottling and Over heating Issues) and these were the results that I got.

## Results
 
#### Validation Set Accuracy : 95.9% 
#### Test Set Accuracy : 95.9%
