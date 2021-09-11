# Spam-Email-Classifier
This LogisticRegression model is built using basic machine learning techniques to classify spam emails. It is a Binary Classifier that only predicts whether an email is HAM or SPAM. The datastet is taken from an open source public database which stores email data for training and research purposes. 

#### SUMMARY
The data is loaded and parsed using python library functions. Custom functions and Transformers are written in the code to transform the loaded data into lowercase plain\text format and all numbers, punctuations or URLs are either removed or replaced with alternate words or same words with their suffixes removed. The emails are converted into vectors of common words that are present in them along with their counts. An ordered list of most common words present in a spam email is built and each email is checked using the list to see how many of these words  are present in the input. If the count is high then the email is marked as SPAM and if not then HAM.

# Libraries used:
- Pandas 
- Numpy
- urlextract
- nltk
- matplotlib
- scikit-learn

# Project Structure
**Branch: Main**
- **datasets\housing** - contains the original data in the easy_ham and spam sub-folders.
- **Spam_classifier.ipynb** - contains all the code used to transform the data and build the model.
- **spam_email.pkl** is the model itself after being trained saved using the joblib function.
