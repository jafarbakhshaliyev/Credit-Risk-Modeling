# Credit-Risk-Modeling
<img width="735" alt="Screen Shot 2022-05-18 at 5 30 07 PM" src="https://user-images.githubusercontent.com/88124269/169166139-9eb7b8b6-f1c4-41e0-9820-85bb4d7c209b.png">


I worked on the project for MaxDecisions Inc. in Richardson, TX, USA. The project is about exploring a small credit risk dataset and applying various advanced Machine Learning algorithms to predict the probability of default for applicants. 

As part of EAD, I looked at some statistics information on each feature and plotted to see how the dataset is imbalanced. After analysis, I dropped the repeated columns, chose continuous numerical columns to scale using Standardization, and applied the oversampling technique to deal with imbalanced data.

I implemented XGBoost, CatBoost, SVM, and basic Neural Networks on the small credit risk dataset. To see the model performances, I used the code which divides the applicants into the bins and show bad rates and average predicted score for each bin. These rank order tables also describe ROC-AUC and KS scores to compare the models. I used the ROC Curve plots for train, test, and in-sample validation datasets to compare the results from each algorithm. In the end, I used swap set analysis to see how the ratio of swap-in per swap-out population, misclassification rate, and false negatives (bad accounts which are treated as good accounts) change according to these four models. 

As a result, we see that XGBoost and Support Vector Machine are performing better results based on scores of ROC-AUC and KS, as well as on swap-set analysis. Our other team members used different models such as Naive Bayes, KNN, and Random Forest, which results from these algorithms are behind the ones from CatBoost, XGBoost, and SVM. Also, basic Neural Networks (and KNN) gave the worst result because of the small credit risk dataset (6358 rows).
