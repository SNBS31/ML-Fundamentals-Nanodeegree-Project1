# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE Salle-Njume Brian Salle

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
That those scores increased in the course of comparing them with other models in Kaggle.
But I was made very aware that Kaggle doesn't accept submissions containing negative values.

### What was the top ranked model that performed?
WeightedEnsemble_L3

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
I splitted the datetime into hour, using the to_datetime().dt.hour conversion.
I also ensured that our computer didn't see our season features as just numbers, but into the category datatype for convinience sake.

### How much better did your model preform after adding additional features and why do you think that is?
After applying EDA and neccessary Feature Engineeriing,our result was 0.44645790695, meaning 44% better.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
The error metric actually reduced,which is a good thing

### If you were given more time with this dataset, where do you think you would spend more time?
How to avoid my model from overfitting, so as to improve it.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|default|default|default|1.80224|
|add_features|default|default|default|0.59469|
|hpo|max_depth|max_features|max_samples|0.48560|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](cd0385-project-starter/project/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.
![model_test_score.png](cd0385-project-starter/project/model_test_score.png.png)

## Summary
This project I was been called upon to do, outlines a complete process for building and assessing a bike-sharing demand prediction model with AutoGluon. It covers essential steps like data preparation, feature engineering, hyperparameter tuning, and submission to Kaggle for evaluation.
It was a wonderful way to get my hands dirty, and gain hands-on experience.