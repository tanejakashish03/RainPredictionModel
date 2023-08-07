# Rain Prediction Model
It is a project on predicting whether it will rain tomorrow or not by using the Rainfall in Australia dataset.

# TechStack
Front-End: HTML, CSS  
Back-End: Flask  
IDE: Google Colab  

# Dependencies
Visual Studio Code  
Google colab research  
numpy  
pandas  
sklearn  
flask-ngrok  
datetime  
render_template  
requests  

# Dataset
Link: https://drive.google.com/file/d/1vqoC-Mm1W9voR36ofj_39D8ig8ekoG9H/view?usp=drive_link  
Description:  
This dataset contains about 10 years of daily weather observations from many locations across Australia.  
Location - Name of the city from Australia.  
MinTemp - The Minimum temperature during a particular day. (Degree Celsius)  
MaxTemp - The maximum temperature during a particular day. (Degree Celsius)  
Rainfall - Rainfall during a particular day. (millimeters)  
Evaporation - Evaporation during a particular day. (millimeters)  
Sunshine - Bright sunshine during a particular day. (hours)  
WindGusDir - The direction of the strongest gust during a particular day. (16 compass points)  
WindGuSpeed - Speed of strongest gust during a particular day. (kilometers per hour)  
WindDir9am - The direction of the wind for 10 min prior to 9 am. (compass points)  
WindDir3pm - The direction of the wind for 10 min prior to 3 pm. (compass points)  
WindSpeed9am - Speed of the wind for 10 min prior to 9 am. (kilometers per hour)  
WindSpeed3pm - Speed of the wind for 10 min prior to 3 pm. (kilometers per hour)  
Humidity9am - The humidity of the wind at 9 am. (percent)  
Humidity3pm - The humidity of the wind at 3 pm. (percent)  
Pressure9am - Atmospheric pressure at 9 am. (hectopascals)  
Pressure3pm - Atmospheric pressure at 3 pm. (hectopascals)  
Cloud9am - Cloud-obscured portions of the sky at 9 am. (eighths)  
Cloud3pm - Cloud-obscured portions of the sky at 3 pm. (eighths)  
Temp9am - The temperature at 9 am. (degree Celsius)  
Temp3pm - The temperature at 3 pm. (degree Celsius)  
RainToday - If today is rainy then ‘Yes’. If today is not rainy then ‘No’.  

# Algorithm Used
Random Forest Classifier   
A random forest classifier is a collection of tree-structured classifiers whose results are compounded into one result; it is an ensemble machine learning algorithm which can be implemented for both classification and regression tasks and is made up of a set of classifiers known as a decision tree (Tin Kam Ho 1998) (Breiman Leo 2001), random forest classifier is known to produce accurate predictions, provides flexibility and reduced the risk of overfitting.

# Working of Model
- The model was trained based on the given dataset using the random forest classifier algorithm.
- Once the training is complete and it has tested the predictions, pickle file is loaded on to the server.
- The pickle file helped me to save the ML model, to minimise lengthy re-training and even allow me to share, commit, and re-load pre-trained rain prediction model to the frontend servers using flask.
- Flask used the saved model to connect the backend with the frontend that inputs the values in the prediction page and thus after few seconds, the provided data will be sent to the backend which will then process it and return a prediction as to whether it will be a rainy or a sunny day.
- This output will directly be shown to the user predicting the occurence of rain.

# Predictor
![predictor](https://github.com/tanejakashish03/RainPredictionModel/assets/140004057/20337e70-5984-4d11-83f2-ed8f20e8ef65)

# Rainy Day
![after_rainy](https://github.com/tanejakashish03/RainPredictionModel/assets/140004057/d049bb68-845b-4393-af3d-13596831e248)

# Sunny Day
![after_sunny](https://github.com/tanejakashish03/RainPredictionModel/assets/140004057/8deb8433-a3d8-4ff1-82d3-9b60adc8b18c)

# Vote of Thanks
Kaggle for providing the dataset, link: https://www.kaggle.com/jsphyg/weather-dataset-rattle-package
