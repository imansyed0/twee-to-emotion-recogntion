A developed approach to recongising emotion/sentiment from tweets. Supervised machine learning. .py files correspond to ml model used.

Problem : Given a dataset mapping tweets to the associated emotions, create an tweet-to-emotion recogniser.

-> Dataset - https://www.crowdflower.com/wp-content/uploads/2016/07/text_emotion.csv

-> Libraries - Natural Language Tool-kit (NLTK) and Sci-kit learn

Pre - processing

-> Removal of regular expressions, symbols using the 're' library

-> Removal of lemmas (Lexicon Normalization) using WordNetLemmatizer from NLTK

-> Removal of multi-letter ambiguities, e.g 'yessss' gets converted to 'yes'

Vectorization

-> Term frequency - inverse document frequency (TfidfVectorizer) deployed for converting the words to vectors (for SVM and Naive Bayes)

-> Bag of words representation used as an input for the sigmoid layers model

Modelling

-> 1. Support Vector Machine - Creation of hyperplanes separating all the classes, linear kernel.

-> 2. Naive Bayes classifier - naively assuming no inter-dependence between words.

-> 3. Aritificial Neural Network - 3 layer neural network.