# Weather-Classification
Predicta 1.0 is an AI prediction challenge competition hosted by the IEEE student branch of the University of Peradeniya. This repository includes my Kaggle submission, which secured 2nd place on the public leaderboard.

Score : 0.921

## Task Overview

The goal was to develop a machine learning model capable of accurately classifying daily weather conditions into predefined categories using historical weather data. It involved extensive data preprocessing, feature engineering, and model evaluation to identify the most effective predictive model.

## Dataset

The dataset (daily_data.csv) used in this task includes various weather-related features such as temperature, humidity, wind speed, atmospheric pressure, precipitation, and more. Categorical variables such as city identifiers were also included, which were crucial for geographical analysis.

## Methodology

### Data Preprocessing

The preprocessing steps included:

- Removing irrelevant columns (e.g., sunrise, sunset)
- Handling missing values in the target variable
- Standardizing numerical features using StandardScaler
- Encoding categorical variables using one-hot encoding

### Feature Selection and Engineering

Key features selected for weather condition classification:

- Temperature in Celsius
- Humidity percentage
- Wind speed and direction
- Atmospheric pressure
- Precipitation and cloud cover
- Interaction terms (e.g., temperature-humidity interaction)
  
### Model Selection and Training

Various classification algorithms were evaluated:

- Ensemble methods (AdaBoost, Bagging, Random Forest, Gradient Boosting)
- Support Vector Machines (SVM)
- Gaussian Processes
- Naive Bayes
- K-Nearest Neighbors
- XGBoost
  
Cross-validation and hyperparameter tuning (via GridSearchCV) were used to optimize model performance. The best-performing model was selected based on accuracy scores and validated using ShuffleSplit cross-validation.

## Results

The Gradient Boosting Classifier emerged as the top-performing model, achieving the highest accuracy in weather condition prediction. Ensemble methods generally outperformed individual classifiers, demonstrating their effectiveness in handling complex weather patterns.
