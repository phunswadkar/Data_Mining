# Data_Mining
Data Mining | Supervised Learning Methods to classify the Quality of Red Wine

## Overview:
Throughout centuries of history, wine has retained its status as a cherished beverage enjoyed across the globe. However, the evaluation of wine quality historically relied on subjective and time-consuming methods. Consequently, our aim was to employ data-driven approaches, including machine learning, to classify wine quality by utilizing measurable physicochemical attributes. 

To achieve this, we analyzed a dataset of red wine samples, conducted data cleaning, partitioned the data, and trained several supervised learning algorithms which include Classification Tree, Ordinal Logistic Regression and Neural Network Model. Our primary objective was to demonstrate the potential of these techniques in classifying wine quality and to gain valuable insights into the physicochemical factors that impact the quality of red wine.

![Image]()

## Data Description:
	•	Fixed Acidity        : Volume of acids in a sample measured in grams per cubic decimeter (g/dm3)
	•	Volatile Acidity.    : Volume of acetic acid in a sample measured by (g/dm3)
	•	Citric Acid          : Used by winemakers in acidification to boost the wine's total acidity measured by (g/dm3)
	•	Residual sugar       : Amount of sugar left after fermentation measured by (g/dm3)
	•	Chlorides            : Amount of salt in wine measured by (g/dm3)
	•	Free Sulfur.         : Amount of unbound sulfur dioxide that inhibits microbial
	•	Dioxide.             : Growth and oxidation measured by milligram per cubic decimeter (mg/dm3)
	•	Total Sulfur Dioxide : Total amount of sulfur dioxide in wine – both free and bound - measured by (mg/dm3)
	•	Density              : Density of the wine measured by gram per cubic centimeter (g/cm3)
	•	pH.                  : pH describes how acidic or basic a wine is
	•	Sulphates.           : Contributes to sulphur dioxide gas, measured by (g/dm3)
	•	Alcohol.             : Percent of alcohol in wine
	•	Quality.             : Categorical value on a scale between 3 and 8, higher values denote higher quality
  
  ## Problem Statement:
  • To be able to classify the quality of wine based on its physicochemical properties.
  
The intended audience for this project includes winemakers, wine experts, and wine sellers. They can use the analysis results to determine which chemical features are important in determining the quality of red wine. The predictions of this project can also help identify the right price for the right quality of wine. In addition, the results can also help stakeholders devise appropriate marketing plans according to the quality of wines.

## The Approach and Machine learning Models used:
Our objective is to classify the quality of red wine which is an ordinal variable represented by quality_category using 11 predictor variables. Since there is a specific target to predict, this task will be considered supervised learning. In order to predict the quality of red wine, We used three different machine learning models: 
• Ordinal Logistic regression model (Specifically, since we have three categories low, medium, and high)
• Classification Tree
• Neural network model
 
 ### Note: 
 To utilize logistic regression for multiclass classification, the categories must be converted into numeric values such as dummy variables (0, 1, 2, etc.), as the logistic function's formula represents the probability of a multiple outcome variable as numeric values, not alphanumeric categories like 'low', 'medium', and 'high'. This project will therefore convert quality variable at two steps – once to convert from numerical to categorical in three levels (high, medium and low) and once to convert alphabetical labels to numeric dummy variables. The three-level dummy variables will be called quality_category_int in the dataframe, and will be used for both logistic regression and neural network model. The results will be compared to identify the most effective model.
 
 ## Result:
 All the three models showcased commendable performance. The classification tree soared above the rest with an impressive 83% accuracy, closely followed by the neural network model, and then the ordinal logistic regression model. These findings imply that any of these three models can effectively forecast the quality of red wine based on predictor variables.

Moreover, our confident recommendation extends to predicting medium quality wines using all three models. However, when it comes to low- and high-quality wines, our enthusiasm is accompanied by caution. To fortify the models' ability to predict these extremes, we suggest enriching the training data with a greater focus on low- and high-quality wines. By doing so, we can bolster the models' predictive prowess and enhance their accuracy for these particular categories.
