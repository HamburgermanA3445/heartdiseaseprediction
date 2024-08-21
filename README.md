# heartdiseaseprediction
Comparison of several classification models for predicting heart disease risk, and for investigating lifestyle factors' effect on heart disease.


1. I found six Kaggle datasets to evaluate over with several classifier models, with Heart Disease as the binary target: Logistic Model, Neural Network from Scratch, TensorFlow, Random Forest (RF), Decision Tree (DT), k-Nearest Neighbors (KNN), Gradient Boosting Machine (GBM), Support Vector Machine (SVM), and Extra Trees (ET). 
2. Of the six datasets, three of them were heavily biased towards classifying patients with no heart disease, as the classification report showed very low or even 0 accuracy in predicting patients with it. 
3. The rest were fine, and I found that ET performed the best (the first dataset said it had a perfect f1 score, meaning it may have overfitted), followed by GBM/RF as the second and third best performing (by f1 score). I looked at the feature importance when using all features to predict, and found that exercise angina and old peak were consistently a part of the highest ranks for all working datasets, with ST_slope being ranked first in two of the working datasets (datasets 3, and 6 at end of the email).
4. I also tested what happens when I remove those features, and surprisingly, the first good dataset (dataset 2) sought a 1% increase in accuracy after removing the lifestyle factors, while the other two good datasets (datasets 3, 6) had a 1-2% decrease in accuracy. 
5. On the other hand, when I removed ST_slope, dataset 2 saw an increase in accuracy by 2%, while datasets 3 and 6 decreased by 3% and 8%, respectively.
