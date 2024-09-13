# Real-estate-house-price-prediction-with-neural-networks

This project explores how to solve regression problems using PyTorch. We focus on predicting a house's price per unit area based on various features such as transaction date, house age, distance to the nearest mass rapid transit station, number of convenience stores, latitude, and longitude. This project demonstrates how to prepare data, build and train a neural network model, and evaluate its performance.

**Project Overview**

House price prediction is a common regression task where the goal is to estimate the value of a property based on multiple input features. This project involves:


- Preparing the dataset for training and testing.
- Building a neural network model using PyTorch.
- Training the model on the dataset.
- Evaluating the model using performance metrics.
- Making predictions and comparing them with actual values.
  
**Dataset**

The dataset contains the following features:

- Transaction date
- House age
- Distance to the nearest mass rapid transit station
- Number of convenience stores
- Latitude and longitude
- The target variable is the house price per unit area.

You can access the dataset here: House Price Dataset https://bit.ly/47KnAH5

**Key Steps**

**1. Data Preparation**

- Load the dataset using Pandas.
- Split the dataset into training and testing sets.
- Convert the data to PyTorch tensors for use in the model.
  
**2. Model Building**

We build a neural network using PyTorch's torch.nn.Module. The model consists of six fully connected layers, designed to learn the relationships between the input features and the target variable. The last layer has no activation function since the task is regression, and we want to predict continuous values.

**3. Model Training**

The model is trained using the Mean Squared Error (MSE) loss function, which calculates the squared difference between the predicted and actual values. We use the Adam optimizer for training, and the model is trained for 1000 epochs.

**4. Model Evaluation**

The model is evaluated using two key metrics:

- **Mean Absolute Error (MAE):** Measures the average absolute difference between the predicted and actual values.
- **Mean Squared Error (MSE):** Measures the average squared difference between the predicted and actual values.
These metrics help to understand the model's performance on the test set.

**5. Visualizing Loss**

To monitor the model’s training progress, we plot the loss values over the epochs, which helps in identifying any anomalies or issues during training.

**6. Making Predictions**

We use the trained model to make predictions on the test set. The results are compared with the actual values, and the model's performance is assessed based on MAE and MSE. Additionally, we perform inference on new data to predict the house price per unit area.

**Results**

- Mean Absolute Error (MAE): 5.16
- Mean Squared Error (MSE): 52.98
  
These metrics indicate that, on average, the model is off by 5.16 units in predicting the price per unit area of a house.

**Conclusion**

The project demonstrates how to effectively use PyTorch to build and train a neural network model for regression tasks. By understanding the data and applying appropriate techniques, we achieve a reasonably accurate model for house price prediction.
