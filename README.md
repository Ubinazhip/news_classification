# news_classification
LSA_classification

The problem from Kaggle: https://www.kaggle.com/c/learn-ai-bbc/ <br>
# Data 
We are given the training set of 1490 samples, with 3 features: Article_id, text, category <br>
There are 5 categories: sport, tech, business, politics, entertainment <br>
We are also given test set of size (735, 2), only 2 features: article_id and text, so we have to classify those texts. <br>

# Method
According to the assignment, I had to use LSA, which is simply getting the vector representations of text and doing Truncated SVD. Truncating SVD really helped to improve the accuracy, since we are picking only the most important part of the information. For classification, we have just used KNearestNeighbor(best hyperparameters were found using gridsearch), which gave a good accuracy of around 96%< on the test set(both private and public).


# Authors
Aslan Ubingazhibov - Data Science, Higher School of Economics, aubinagzhibov@edu.hse.ru <br/>
# Reference
https://www.machinelearningplus.com/nlp/lemmatization-examples-python/ <br>
https://github.com/chrisjmccormick/LSA_Classification/blob/master/runClassification_LSA.py <br>
https://www.kaggle.com/c/learn-ai-bbc/data <br>
https://www.engr.uvic.ca/~seng474/svd.pdf
