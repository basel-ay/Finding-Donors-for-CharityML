# Finding-Donors-for-CharityML

<p align="center">
  <img src="https://user-images.githubusercontent.com/64821137/196411661-cc980bc7-8e29-45ad-b1b9-33cde9b457cd.png"/>
</p>

CharityML is a fictitious charity organization located in the heart of Silicon Valley that was established to provide financial support for people eager to learn machine learning. After nearly 32,000 letters were sent to people in the community, CharityML determined that every donation they received came from someone that was making more than $50,000 annually. To expand their potential donor base, CharityML has decided to send letters to residents of California, but to only those most likely to donate to the charity. With nearly 15 million working Californians, CharityML has brought you on board to help build an algorithm to best identify potential donors and reduce overhead cost of sending mail. Your goal will be evaluate and optimize several different supervised learners to determine which algorithm will provide the highest donation yield while also reducing the total number of letters being sent.

## Dataset 

The dataset for this project originates from the UCI Machine Learning Repository. The datset was donated by Ron Kohavi and Barry Becker, after being published in the article "Scaling Up the Accuracy of Naive-Bayes Classifiers: A Decision-Tree Hybrid". You can find the article by Ron Kohavi online. The data we investigate here consists of small changes to the original dataset, such as removing the 'fnlwgt' feature and records with missing or ill-formatted entries.

![image](https://user-images.githubusercontent.com/64821137/196415446-5c86129c-7a17-4d1d-8731-b9df69cf0e91.png)

## Supervised Learning Models

The following are some of the supervised learning models that are currently available in `scikit-learn`:
* Logistic Regression
* Decision Trees
* K-Nearest Neighbors

![image](https://user-images.githubusercontent.com/64821137/196415997-d4c9682e-7667-4053-a53a-da24bf758707.png)

## Model Tuning

Fine tune the chosen model. Use grid search (GridSearchCV) with at least one important parameter tuned.

![image](https://user-images.githubusercontent.com/64821137/196416210-55403b67-35b8-4a90-bc48-6d9b14ba34a2.png)

## Feature Importance

An important task when performing supervised learning on a dataset like the census data we study here is determining which features provide the most predictive power. By focusing on the relationship between only a few crucial features and the target label we simplify our understanding of the phenomenon, which is most always a useful thing to do. In the case of this project, that means we wish to identify a small number of features that most strongly predict whether an individual makes at most or more than $50,000.

Choose a scikit-learn classifier (e.g., adaboost, random forests) that has a feature_importance_ attribute, which is a function that ranks the importance of features according to the chosen classifier. fit this classifier to training set and use this attribute to determine the top 5 most important features for the census dataset.

![image](https://user-images.githubusercontent.com/64821137/196416499-4d5e0546-c391-4d9c-a2c4-9e5ac50cef76.png)

