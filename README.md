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
pickle  
sklearn  
flask-ngrok  
datetime  
render_template  
requests  

# Dataset
Link: https://drive.google.com/file/d/1vqoC-Mm1W9voR36ofj_39D8ig8ekoG9H/view?usp=drive_link  

# Algorithm Used
Random Forest Classifier   
A random forest classifier is a collection of tree-structured classifiers whose results are compounded into one result; it is an ensemble machine learning algorithm which can be implemented for both classification and regression tasks and is made up of a set of classifiers known as a decision tree (Tin Kam Ho 1998) (Breiman Leo 2001), random forest classifier is known to produce accurate predictions, provides flexibility and reduced the risk of overfitting.

# Working of Model
The model was trained based on the given dataset using the random forest classifier algorithm.
  ### Model Training
  - Import libraries stated in the dependencies.
  - The dataset is imported and encoded, ensuring that invalid data is dealt with.
  - The encoded dataset is then splitted into training set and test set.
  - The training set is used to train the model using classifier algorithm and predictions are made on the test set.
  - Pickle file of trained model is then created and saved.
  ### Model Deployment using Flask
  - This pickle file is loaded by app.py in which the flask model will request input parameters from the user.
  ### Predictor
![predictor](https://github.com/tanejakashish03/RainPredictionModel/assets/140004057/20337e70-5984-4d11-83f2-ed8f20e8ef65)
  - These input parameters are then loaded by the model and prediction is made.
  - These predictions are sent to flask server which will process it and the output is directly shown to the user as to whether it will be a rainy or a sunny day.

# Rainy Day
![after_rainy](https://github.com/tanejakashish03/RainPredictionModel/assets/140004057/d049bb68-845b-4393-af3d-13596831e248)

# Sunny Day
![after_sunny](https://github.com/tanejakashish03/RainPredictionModel/assets/140004057/8deb8433-a3d8-4ff1-82d3-9b60adc8b18c)

# Vote of Thanks
Kaggle for providing the dataset, link: https://www.kaggle.com/jsphyg/weather-dataset-rattle-package
