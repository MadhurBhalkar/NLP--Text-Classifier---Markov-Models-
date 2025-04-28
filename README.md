# NLP--Text-Classifier---Markov-Models-

I will be applying the concept of Maekov Model in an supervised context 

--Bayes Classifier---

Two sets of Poems from different authors:
Peoms by Robert Forst
Poems by Edgar Allan Poe 

Bayes' Rule is applied to 
Compute the probability of poem belonging to a certain atuher
Each model was trained on data by a specific author 


I have used Markov Models for text classification by creating a separate model for each class 
Markov Models are used to compute the likelihood of probability for each class 
Bayes Rule is used as the decision rule 
Since all classes have an equal chance of being chosen ..making it a simple problem of maximum likelihood…hence we will be leveraging the MAP method


Involves Building two seeprate markov models 
Test how well the model performs by computing train and test accuracy
To check for class imbalance F1 score is used 

***Code Explanation 

*each line of each poem is considered a sample for our ML Model 
*save lables 
*train test Split
*input is lines of text---- we will implement a markov transition matrix -- mapping from uniique word to unique integer intext
Tokenize each line of text  using a string split 
Assign unique words a unique index
Mapping -- refer to python dictionary
Special index for unknowns 
Word to Integer Index Mapping

Convert each line of text into interger lists 
Train a Maekov model for each classe (Edgar Allan Poe/ Robert Frost )
TO apply Baye's rule ,we will compute Priors for each class 


**Code Details 
Write a function to make prediction 
Take input sequence and compute postetort for each class
Makr predictions for train and test 
Check for imbakace
Confusion matrix
F1 score 
