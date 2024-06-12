# Air Quality Prediction

# Project Overview
This project focuses on monitoring and understanding air quality, which is essential for our wellbeing. The aim is to assess air quality in Indian cities by predicting the Air Quality Index (AQI) based on vehicular and industrial pollution contents using machine learning models. This work incorporates earth observation practices.

# Dataset
The air quality dataset, adapted from a previous dataset by Rohan Rao, includes daily level data collected from various stations across multiple cities in India. The dataset is divided into three parts:

-Training Set: 17,395 samples for training and optimizing the model.
-Validation Set: 1,491 samples for evaluating the model locally.
-Testing Set: 5,964 samples for testing the model performance on unseen data (no target variable included).
## Variables
-City: City identifier.
-Date: Date of data collection.
-Vehicular Pollutants:
-PM2.5: Fine inhalable particles (≤2.5 micrometers).
-PM10: Inhalable particles (≤10 micrometers).
-NO: Nitric oxide concentration.
-NO2: Nitrogen dioxide concentration.
-NOx: Nitrogen oxides concentration.
-NH3: Ammonia concentration.
-CO: Carbon monoxide concentration.
-Industrial Pollutants:
-SO2: Sulphur dioxide concentration.
-O3: Ozone concentration.
-Benzene: Benzene concentration.
-Toluene: Toluene concentration.
-Xylene: Xylene concentration.
-Air Quality: Designation of air quality (Moderate, Satisfactory, Poor, Very Poor, Good, Severe).
-AQI: Air Quality Index (target variable).

# Data Cleaning and Preprocessing
-Handling Missing Values: NaN values were filled.
Encoding Categorical Variables: Categorical variables were encoded using a label encoder.
-Feature Extraction: Relevant features were extracted to enhance the model performance.

# Modeling
This is a regression task aimed at predicting the AQI. A Random Forest model was trained using the training data. The model was then validated using the validation set and evaluated for inference.

# Evaluation Metric
Log Root Mean Squared Error (LRMSE) was used to evaluate the model performance. LRMSE is less sensitive to the scale of the target variable compared to RMSE and penalizes large differences between predicted and actual values. The model achieved an LRMSE score of 3.677.

# Prediction
The test data were used to predict the Air Quality Index in various Indian cities.

# Conclusion
Through this experiment, it was found that both vehicular and industrial pollution content significantly contribute to the Air Quality Index (AQI) in Indian cities. This model can be used to monitor and predict air quality, providing valuable insights for environmental and public health planning.
