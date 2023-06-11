# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Aveenash

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
-  Specifically, I realized that negative count values should be rounded down to zero. Additionally, I understood that the numbers within the count column should be rounded to zero. These changes were necessary to ensure the accuracy and consistency of the submitted results.
### What was the top ranked model that performed?
WeightedEnsemble_L3

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
- During the exploratory analysis, it was discovered that the demand varied throughout the day on weekdays and weekends. This insight led to incorporating time series analysis to capture the changes in demand within each hour. urthermore, continuous features such as temperature, humidity, and wind were categorized, likely to enhance the model's performance.
- 
### How much better did your model preform after adding additional features and why do you think that is?
The model's performance saw a significant enhancement of around 20% after incorporating the additional features. The improvement can be attributed to the inclusion of relevant features based on domain knowledge. By considering factors such as the time of day and weather conditions, the model can make more accurate predictions.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
A slight improvement in the kaggle score has been found after changing the hyper parameters.

### If you were given more time with this dataset, where do you think you would spend more time?


### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score (1).png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_sfcore.png](img/model_test_score (1).png)

## Summary
In this project, we have obtained/explored following steps in the ML Lifecycle.

The key objective of the project is to leverage the data generated by bike sharing systems, along with external information, to optimize business outcomes. The data, obtained from the "Bike Sharing Demand" Kaggle competition, undergoes thorough analysis, visualization, and modifications using popular Python libraries such as Pandas, Matplotlib, and Seaborn. Model development is conducted using the Autogluon AutoML library, initially starting with a model without preprocessing, followed by the creation of new features and hyperparameter tuning. To evaluate the models, predictions are submitted to Kaggle, and their performance is compared based on the obtained scores. This iterative process aims to enhance the accuracy of bike sharing demand predictions and maximize the potential business advantages for firms in the industry.
