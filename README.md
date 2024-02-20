# Predict-Online-Shoppers-Intention

We first fit logistic regression(Model1), regression tree(Model2), and XGBoost(Model3) to the training set, and predict the probability of default for the loans in the validation set. <br>

Next, we try different ensemble models to combine these base model predictions: weighted average (Model4), regression tree stacking (Model5) and XGBoost stacking (Model6). The accuracy is measured by the Brier Skill Score (higher BSS indicates more accurate predictions).

We find that stacking model-XGBoost (Model6) is our best model. Then, we retrain the entire training set using the best model, and generate predictions in the testing set.
