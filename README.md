# Analytics-Vidya-Hackathon
This repository shows my approach and submission for Analytics Vidya Jobathon June'22 comeptition. 

### Problem Statement
We are given a dataset containing leads information. Leads are potential buyers that company has acquired through offline or online campaigns. The main aim is to make a model that will accurately predict if a lead will buy a product from them in the next three months.

A brief summary of my approach is presented here. For more detailed view, feature engineering and EDA please check the python notebook.
### The Dataset
<b>Variables                  Meaning</b><br>
id<t>                            Id of each lead<br>
created_at                    Date the lead was dropped<br>
campaign_var_1                Variable telling us about the campaign related to lead<br>
campaign_var_2                Similar variable<br>
products_purchased            Number of products the lead has purchased in the past<br>
signup_date                   Date the lead signed up on the website<br>
user_activity (12 variables)  Variables showing activity of the user on the website<br>
buy                           The target variable, if the lead buys a product within the next 3 months<br>

### Model Selection & Hyperparameter Tuning
Looking at the distribution of data some models were selected like Random forest, Xgb, SVC with non linear kernel and knn for testing. Then after compairing the f1 score of all the models Random forest was selected and further tuned to get a final score of ~0.93.
![](Images/Screenshot (667).png)
