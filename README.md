# Fashion Product Reviews Analysis 🛍️

## Overview of project
This project is centered around analyzing fashion product reviews to predict ratings and recommendations. Utilizing deep learning techniques, the project delves into the nuances of customer feedback to derive meaningful insights.

## Prediction targets
* Rating Prediction: Uses deep learning models to predict the ratings of fashion products based on customer reviews.
* Recommendation Prediction: Analyzes the text of reviews to predict whether a product is recommended by the reviewer.

## Data components🌟
* Id: Review Id
* Age: Positive Integer variable of the reviewers age.
* Review_Title: String variable for the title of the review.
* Review: String variable for the review body.
* Pos_Feedback_Cnt: Positive Integer documenting the number of other customers who found this review positive.
* Division: Categorical name of the product high level division.
* Department: Categorical name of the product department name.
* Product_Category : Categorical name of the product class name.
* Rating: Positive Ordinal Integer variable for the product score granted by the customer from 1 Worst, to 5 Best. This is one of the target columns.
* Recommended: Binary variable stating where the customer recommends the product where 1 is recommended, 0 is not recommended. This is one of the target columns.

## Performance metrics🔍
Mean Columnwise Spearman's Rank Correlation Coefficient is used for the evaluation the predictions.  This means that for each of the two target variables ("Rating" and "Recommended"), Spearman's Rank Correlation Coefficient is calculated between the prediction and the ground truth, and the result is averaged for the two columns to give the final score.

This means that scores range between -1 and 1, with bigger scores being better.
