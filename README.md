# Predicting Housing Prices with Machine Learning

## Introduction 
In the real estate sector, accurate house price prediction is a complex yet valuable challenge. It can assist buyers and sellers in making informed decisions, as well as help real estate professionals analyze market trends. This study focuses on applying two machine learning models to solve this problem: Linear Regression and Decision Tree. The objective is to compare the performance of these two models to determine which is more suitable for the selected dataset.
This study has developed a model capable of predicting housing prices using Machine Learning. The model delivers predictions with about 61% accuracy. The model relies on historical data such as area, bedrooms, bathrooms, stories, parking, and more. I researched and tested several Machine Learning algorithms to select the one that maximizes prediction accuracy.

## Methodology & Results
To answer the research question, I apply the training/test method with two models as Linear Regression and Decision Tree with pruning. After running the models, I will choose and pick the best model based on the accuracy score. 

The analysis is designed to achieve three goals:

- The first thing establish a baseline model using Linear Regression to calculate the contribution of property attributes as area, bedrooms, bathrooms, and stories to housing prices.
- The second thing implement a more flexible predictive model using a Decision Tree with pruning to capture non-linear relationships and interactions between features while controlling for overfitting.
- The final thing compare and interpret results to assess trade-offs between model interpretability and predictive power, thereby providing actionable insights for practical decision-making.

To predict housing price, I apply three model’s Linear regression, Decision tree with pruning. 

## Model selection
**Table 2:** Training/Testing performance (R2, RMSE, MAE).

| Model              | Train R²        | Test R²         | Test MSE   | Test MAE  |
|--------------------|-----------------|-----------------|-------------|-----------|
| Linear Regression  | 0.699 (69%)     | 0.588 (58%)     | 1,211,349   | 849,809   |
| Decision Tree      | 0.732 (73%)     | 0.333 (30%)     | 4,870,169   | 1,085,615 |

The results indicate that Linear Regression achieved better generalization, with a test R2 of 0.588 (58%), compared to 0.333 (33%) for the Decision Tree with pruning. Although the Decision Tree obtained higher training performance (R2 = 0.733 (73%)), the sharp drop in the test set shows clear signs of overfitting. In contrast, Linear Regression maintained more consistent performance across training and testing.

## Conclusion and future works
In this study, we limited our scope to comparing Linear Regression and a pruned Decision Tree on a relatively small housing dataset. However, the same methodology could be applied to larger and more diverse datasets, as long as sufficient and reliable data are available. The factors we identified as impactful for predicting housing prices, such as property size, location attributes, and amenities, remain relevant across different regions and markets. 

Based on the current analysis, several directions can improve result predictive performance. Future work could include applying a transformation to the target variable as using a log transformation, which I think will help reduce heteroscedasticity and improve the fit of Linear Regression.





