# Sentiment-Analysis---Selecting-the-best-company-with-most-positive-number-of-reviews
This project aims at using sentiment analysis to classify the positive, negative and neutral amazon reviews associated to various android applications based on their class labels (1 - Negative review, 2 - Neutral review, 3 - Positive review).

The training and testing datasets are are provided as 'Train dataset' and 'Test dataset' with 20,000 and 19,999 reviews each respectively, in the repository. Each review, in both training and test datasets, consists of: a) the review text as provided by an Amazon customer, b) a class label with values 1 (negative review), 2 (neutral review) and 3 (positive review) and c) the ID code of the corresponding Android application.

We employ various classification models such as Decision Tree (DT) Classifier, K-Nearest Neighbour (KNN), Support Vector Machines (SVM) and Random Forest Classifiers (RFC) to compare and analyse which algorithm works best in classifying the Amazon reviews relevant to android applications, under their appropriate labels. Evaluating the prediction accuracy scores for each model implemented, we choose the prediction results of the best performing model, to check which Android Application Development Company is likely to achieve profitable returns depending on the class labels of the applications they own. We use Python programming and Jupyter Notebook environment to build this software. The companies and their corresponding applications are provided in the 'Companies and applications.png' file of the repository.


Among the four models implemented, evaluating the classification report and analysing the best performing model using cross-validation, we conclude that the Random Forest model performed efficiently well and was less time consuming while predicting results. Although the f1-score and average test accuracy of the SVM algorithm was slightly better than that of RFC, the time consumed by SVM to predict the test results were a lot more than that taken by the RFC. In addition to this, the precision values of RFC are higher than SVM precision values and for problems involving multiple classes and sentiment analysis based on online data, RFC works better than the SVM.

After performing Sentiment Analysis we concluded the following:

1) We achieved a 75% accuracy and higher values of precision (Negative review – 62%, Neutral review – 47%, Positive review – 76%) for RFC compared to the other classifier algorithms.

2) Using the prediction results of RFC we checked for the most successful company that is capable of providing ROI.

3) Critically evaluating the test reviews for applications relevant to AAD_1 and AAD_2, we notice that the data provided for AAD_1 is not enough and hence we need more data on its corresponding application reviews to confirm which of the two companies are more successful. Since we do not have the required data for AAD_1 at hand, we conclude that AAD_2 is more successful.
