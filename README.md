# Argument-Effectiveness-Analysis
Using NLP to find the best way to rate an argument

There are Two Notebooks:
1. NLP_Project: Here I used Transformer model BERT and added a simple NN on top to classify the arguments
2. NLP_Embeds_and_Classifiers: Here I extracted all the embeddings of input using BERT and then added custom classifiers on top.

The Neural Network and Logistic Regression gave the same overall accuracy but NN could not classify ineffective arguments but LR had a better F1 Score.
