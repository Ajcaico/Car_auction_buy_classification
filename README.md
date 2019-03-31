# Car_auction_classification

This was created for my Data Mining class at Carnegie Mellon. This is based on the "Don't get kicked" Kaggle competition.
Objective: Predict whether a car bought at an auction by a car dealer will be a good buy or bad buy. A bad buy, called a lemon, is when a car has unforseen problems and is worth less than the auction price paid.

Method: Exploratory data analysis was conducted on the data and the features. Data transformation was performed to clean and standardize the data (more information in the HTML analysis report file). The exploratory data analysis shows that there is a skewed distribution of the values of the target variable. There are 12.3% “BadBuys” in the overall data. It is more important to correctly to predict “BadBuys”. To account for this, we used down sampling and true class probs when training the model. Several models are being assessed for this binary classification problem -CART -Bagged CART -Naive Bayes -GCV MARS Earth. These models where each assesed by tuning their respective hyperparameter grid using cross validation. The evaluation metric used was area under the ROC curve (AUC-ROC). The Multivariate Adaptive Regression Splines (MARS) model performed the best with AUC-ROC value of 0.73.

Full analysis in HTML file.
