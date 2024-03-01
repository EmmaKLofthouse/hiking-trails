# Hike Duration Prediction Project

## Overview

This project aims to predict the duration of hikes using data from user reviews. We explore various tree-based machine learning models and ultimately choose XGBoost as the final model. The project involves preprocessing, feature selection, manipulation, hyperparameter tuning, and learning curve analysis to investigate and reduce overfitting, culminating in the production of a final predictive model. The model's performance is evaluated on a separate unseen test sample, and the results are visualized through scatter plots.

## Dataset

The dataset comprises user reviews of hikes from hikr.org, along with associated data such as hike length, elevation, difficulty, start/end times, and the target variable, hike duration. The data was collected and prepared by @roccoli and we download it from the kaggle site at:  https://www.kaggle.com/datasets/roccoli/gpx-hike-tracks/data



## Methodology

1. **Data Cleaning**: We apply further cleaning and processing to remove any inconsistencies or missing values from the data.

2. **Preprocessing and Feature Engineering**: We perform preprocessing steps such as encoding categorical variables, handling missing values, and scaling numerical features.
   
3. **Model Selection**: Various tree-based machine learning models are explored, including Decision Trees, Random Forest, and XGBoost. XGBoost is selected as the final model due to its superior performance.

4. **Feature Importance** We analyse the importance of the features and select those that contribute the most in order to improve the efficiency of the model   

![feature_importance](https://github.com/EmmaKLofthouse/hiking-trails/assets/18194748/5e70c816-a3c2-493e-878f-8d7b0d6b4980)

6. **Hyperparameter Tuning**: Hyperparameters of the XGBoost model are tuned using Hyperopt, a bayesian optimization technique.

7. **Learning Curve Analysis**: Learning curves are analyzed to evaluate the model's performance as a function of training data size and detect any signs of overfitting.
   
![alpha](https://github.com/EmmaKLofthouse/hiking-trails/assets/18194748/336aea8c-51de-4d46-8c15-baa4f67ed5e8)

9. **Evaluation on Unseen Test Data**: The final trained model is evaluated on a separate unseen test sample to assess its generalization performance.


## Results

The XGBoost model demonstrates promising performance in predicting hike durations. Through extensive preprocessing, feature engineering, hyperparameter tuning, and learning curve analysis, we successfully mitigate overfitting and improve the model's ability to generalize to unseen data. The scatter plot of the model's predictions on the test data provides visual confirmation of its predictive accuracy.

   
![final_scatter](https://github.com/EmmaKLofthouse/hiking-trails/assets/18194748/1f9d4bd9-805a-4adc-9a97-eee1e41ac7a0)

## Conclusion

The project showcases the effectiveness of tree-based machine learning models, particularly XGBoost, in predicting hike durations based on user reviews and associated data. The project's methodologies and findings can be extended to other predictive modeling tasks in similar domains. We discuss methods to improve the results, in particular, the option of obtaining or scraping more data could potentially significantly improve the model and help mitigate the issues faced with overfitting.
