## Boston-Housing-Price-Prediction

#### Following points are taken into consideration while making the model.
1. Regression is done using different loss functions than what we used for classification. Mean squared error (MSE) is a loss function commonly used for regression.
2. Similarly, evaluation metrics to be used for regression differ from those used for classification; naturally, the concept of accuracy doesn’t apply for regression. A common regression metric is mean absolute error (MAE).
3. When features in the input data have values in different ranges, each feature should be scaled independently as a preprocessing step(i.e. I am using mean normalization with mean=0, std=1)
4. When there is little data available, using K-fold validation is a great way to reliably evaluate a model.
5. When little training data is available, it’s preferable to use a small network with few hidden layers (typically only one or two), in order to avoid severe overfitting.
#### Model Architecture 
1. I am using Keras Deep Learning Framework for easy implementation.
2. Two Hidden Layers with 64 neuron in each layer.
3. Relu Activation is used for each hidden layer. 
4. As this is regression problem rather than classification, i am using linear activation in final layer. Hence, the network is free to learn to predict values in any range.
5. With **training_data = 404 samples**, **test_data = 102 samples**, I got **MAE 2.5712** which mean my predictions is off by $2571 on average.
