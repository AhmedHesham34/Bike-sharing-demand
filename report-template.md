# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### AHMED HESHAM

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: that i must remove the negative values

### What was the top ranked model that performed?
TODO: The model with hyperparameters (WeightedEnsemble_L3)

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: adding more features in my case doesn't help in decreasing the score but i think in some other cases it may be better.

### How much better did your model preform after adding additional features and why do you think that is?
TODO: actually it is worse, it should've been better but seams like i have to choose differen feature for example (1.977)

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: better than the previous one.(0.477)

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: in choosing the correct hyper parameters

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|default vals|default vals|default vals|1.84700|
|add_features|default vals|default vals|default vals|1.97554|
|hpo|nn_options = {  'num_epochs': 10, 'learning_rate':[1e-4, 1e-2, default=5e-4], 'activation': ['relu', 'softrelu', 'tanh'],  'dropout_prob': [0.0, 0.5, default=0.1], |gbm_options = { 'num_boost_round': 100,  'num_leaves': [lower=26, upper=66, default=36],|default vals|0.47708|

### Create a line plot showing the top model score for the three (or more) training runs during the project.
(It is done in the notebook code)
TODO: Replace the image below with your own.

![2022-07-22_20h28_26](https://user-images.githubusercontent.com/85734497/180501459-3eea4db6-eacb-4a5e-a69c-9501698c6964.png)


### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.
![2022-07-22_07h06_13](https://user-images.githubusercontent.com/85734497/180369888-e49c5ba1-bd22-4846-9ed3-917e9e9ce01c.png)




## Summary
TODO: overall what I learned is that feature engineering is not as important as the hyperparameters as it didn't change the score for better. The hyper parameters are very good as it improved the score more.
