# Argument Effectiveness Analysis
We have used various state-of-the-art Natural Language Processing Techniques to determine the strength of an argument.

Writing is crucial for success. In particular, argumentative writing fosters critical thinking and civic engagement skills, and can be strengthened by practice. However, only 13 percent of eighth-grade teachers ask their students to write persuasively each week. Additionally, resource constraints disproportionately impact Black and Hispanic students, so they are more likely to write at the “below basic” level as compared to their white peers. An automated feedback tool is one way to make it easier for teachers to grade writing tasks assigned to their students that will also improve their writing skills.

This was intended as our solution to a compeition posted on Kaggle. 

## Dataset
The Dataset can be found here: https://www.kaggle.com/competitions/feedback-prize-effectiveness

The dataset presented there contained argumentative essays written by U.S students in grades 6-12. These essays were annotated by expert raters for discourse elements commonly found in argumentative writing:

* Lead - an introduction that begins with a statistic, a quotation, a description, or some other device to grab the reader’s attention and point toward the thesis
* Position - an opinion or conclusion on the main question
* Claim - a claim that supports the position
* Counterclaim - a claim that refutes another claim or gives an opposing reason to the position
* Rebuttal - a claim that refutes a counterclaim
* Evidence - ideas or examples that support claims, counterclaims, or rebuttals.
* Concluding Statement - a concluding statement that restates the claims

Our task was to predict the quality rating of each discourse element. Human readers rated each rhetorical or argumentative element, in order of increasing quality, as one of:

* Ineffective
* Adequate
* Effective

## Our Repository
There are Two Notebooks:
1. NLP_Project: Here We used Transformer model BERT and added a simple NN on top to classify the arguments
2. NLP_Embeds_and_Classifiers: Here we extracted all the embeddings of input using BERT and then added custom classifiers on top.

The Neural Network and Logistic Regression gave the same overall accuracy but Neural Network could not classify ineffective arguments but Logistic Regression had a better F1 Score.

## Results
### 1. Purely BERT
![image](https://github.com/omkmorendha/Argument-Effectiveness-Analysis/assets/17925053/b47a34f0-1931-4067-9f16-e3879fd9f59e)

### 2. BERT + SVC
  ![image](https://github.com/omkmorendha/Argument-Effectiveness-Analysis/assets/17925053/c9bb36bc-bd48-4253-94f4-a1582b35677e)
  
### 3. BERT + LR
  ![image](https://github.com/omkmorendha/Argument-Effectiveness-Analysis/assets/17925053/02951cb7-99fb-44e0-81ba-0a816216e2e5)

### 4.BERT + KNN
  ![image](https://github.com/omkmorendha/Argument-Effectiveness-Analysis/assets/17925053/e165eadd-9ce2-4877-b0d3-66c01a3b76ec)
