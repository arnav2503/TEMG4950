# TEMG4950
This repository has an assignment for TEMG4940:

This machine learning project aims to predict whether a customer will purchase a product or not based on their demographic and behavioral data through the effectiveness of marketing campaigns. The project uses a binary classification model based on Linear Support Vector Classification (LinearSVC) to predict the target variable. It also uses other models to check the data relation. 

The dataset was provided and is split into training, and testing sets with an 80-20 ratio, respectively. The splitting is done randomly, but stratified to maintain the class balance in each set.


The model used in this project is a linear support vector classification (LinearSVC) model, implemented using the scikit-learn library in Python. The model is trained on the training set using default hyperparameters, except for the C parameter which is tuned using a grid search with cross-validation on the validation set. The best C value is chosen based on the F1 score, which is a harmonic mean of precision and recall.

The model is evaluated on the testing set using several metrics, including accuracy, precision, recall, F1 score, and area under the ROC curve (AUC-ROC). The model's performance is also visualized using a confusion matrix, a precision-recall curve, and a ROC curve.


The results of the model show that it achieves an accuracy of 0.67, a precision of 0.65, a recall of 0.71, an F1 score of 0.68, and an AUC score of 0.75 on the testing set. These metrics indicate that the model performs reasonably well in predicting whether a customer will purchase a product or not, based on their demographic and behavioral data, as well as the effectiveness of marketing campaigns.

The confusion matrix shows that the model correctly identifies 58 positive examples (true positives) and 55 negative examples (true negatives), but also misclassifies 30 negative examples as positive (false positives) and 23 positive examples as negative (false negatives).

The precision-recall curve and the ROC curve show that the model has a trade-off between precision and recall, and between true positive rate and false positive rate, respectively. The curves also show that the model outperforms a random classifier, which would have an AUC-ROC of 0.5.

In conclusion, this machine learning project demonstrates the use of LinearSVC for customer analysis and product purchase prediction. The project shows that the model can achieve reasonable performance on a synthetic dataset based on demographic and behavioral data and marketing campaign results. The project also highlights some of the limitations and challenges of using LinearSVC, such as the sensitivity to outliers, the need for hyperparameter tuning, and the requirement for feature engineering and selection. Future work could include exploring alternative models, applying the model to real-world datasets, and integrating the model into a business application.
