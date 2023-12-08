# AutoPartner 🚘
The main goal of this project is to create a blending algorithm with a twist of my own: a dense neural network (DNN), and to do it without any external libraries (i.e. no TensorFlow and no Scikit-Learn).

Autopartner is a machine-learning model that can help a car salesperson predict the ideal price to sell. I used Scikit-learn, TensorFlow, Keras, Pandas, NumPy, and Matplotlib in this project. In this project, I first trained various Scikit-learn models and evaluated them. Afterward, I selected the best models to create a multi-layered perception (MLP). In the end, I created a blending algorithm that ensembles 4 models, and study them with DNN, managing to earn an error (MAPE) of 7,6%, better than the best performing scikit-learn ensemble model (Random Forest Regressor) of 11.6%.

The image below displays the MAPE of several models
![image](https://drive.google.com/uc?export=view&id=1-5a_8IKvEam7R6wct5KADosHwBN6in2H)
Description:
1. Best NN with TensorFlow: A DNN with 3 hidden layers and 6 inputs, or 6 models blended, which are Linear Regression, Random Forest Regressor, K-Nearest Neighbours Regressor, and XGBoost Regressor. With Leaky ReLU.
2. Best NN without TensorFlow: An artificial neural network (ANN) with 3 inputs, or 3 models blended, which are Random Forest Regressor, K-Nearest Neighbours Regressor, and XGBoost Regressor. With ReLU.
3. Random Forest Regressor: Just a normal random forest regressor
4. Improved Blending: An MLP with 3 inputs, or 3 models blended, which are Random Forest Regressor, K-Nearest Neighbours Regressor, and XGBoost Regressor. With ReLU. There's no activation function, i.e. just a linear activation.
5. Original Blending algorithm: An MLP with 6 inputs, or 6 models blended, which are Support Vector Machines, Linear Regression, Random Forest Regressor, K-Nearest Neighbours Regressor, and XGBoost Regressor. With ReLU. There's no activation function, i.e. just a linear activation.
