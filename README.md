# Fashion-MNIST-Image-Classification

## Google Colab Link: https://colab.research.google.com/drive/1Byeh5CcUiAWsBb0PbwlRHVDvfrN-pqYJ?usp=sharing

##Questions:
### 1. What is the Fashion MNIST dataset?
Answer: The Fashion MNIST dataset is a collection of 70,000 grayscale images of clothing items such as shirts, shoes, bags, and coats. Each image is 28×28 pixels and belongs to one of 10 categories. It is commonly used to train and test machine learning models, especially for image classification tasks, as a modern alternative to the original MNIST digit dataset.
### 2. Why do we normalize image pixel values before training?
Answer:We normalize image pixel values to scale them to a range between 0 and 1. This helps the neural network train faster and more efficiently, improves numerical stability, and prevents large pixel values from slowing down or negatively affecting the learning process.
### 3. List the layers used in the neural network and their functions.
Answer:
Flatten layer – Converts the 2D image (28×28 pixels) into a 1D array so it can be processed by the neural network.
Dense (hidden) layer – Learns patterns and features from the input data using neurons and activation functions (such as ReLU).
Dense (output) layer – Produces the final classification output, usually with 10 neurons (one for each clothing category) using the Softmax activation function.
### 4. What does an epoch mean in model training?
Answer: An epoch means one complete pass of the entire training dataset through the neural network. During each epoch, the model learns and updates its weights to improve accuracy.
### 5. Compare the predicted label and actual label for the first test image.
Answer: The predicted label is the category that the model thinks the image belongs to, while the actual label is the true category from the dataset. If both labels are the same, the prediction is correct; if they are different, the model made an error.
### 6. What could be done to improve the model's accuracy?
Answer:Model accuracy can be improved by:
Adding more hidden layers or neurons
Training for more epochs
Using a different optimizer or learning rate
Applying data augmentation
Using a more advanced model such as a Convolutional Neural Network (CNN)

# What is the Fashion MNIST dataset?
Based on my experiment, the Fashion MNIST dataset is a collection of grayscale images used for training and testing an image classification model. Each image has a resolution of 28×28 pixels and represents different clothing items such as:

Shirts
Shoes
Trousers
Bags
I used this dataset to observe how well a neural network can classify clothing images. Compared to the original MNIST dataset, Fashion MNIST is more challenging because it contains more complex and realistic image patterns.

# Data Preprocessing
Why do we normalize image pixel values before training?
In my observation, We normalized the image pixel values by dividing them by 255 so that all values are within the range of 0 to 1. This helped make the training process more stable and faster.

## Normalization allowed the model to:

Update its weights more efficiently
Prevent large pixel values from negatively affecting the learning process
Model Architecture
Layers used in the neural network
Layer	Function
Flatten	Converts the 28×28 image into a one-dimensional array so it can be processed by the neural network
Dense (Hidden)	Uses ReLU activation to learn important features from the images
Dense (Output)	Contains 10 neurons corresponding to the 10 clothing categories in the Fashion MNIST dataset

# Training Process
What does an epoch mean in model training?
An epoch refers to one complete pass of the entire training dataset through the model.

In my experiment, training the model for several epochs allowed it to:

Gradually improve its accuracy
Reduce its loss
By observing the changes in accuracy per epoch, I was able to see how the model learned over time.

# Results
Comparing predicted and actual labels
Based on my results, the predicted label for the first test image matched the actual label provided in the dataset.

## This indicates that:

The model was able to correctly classify the image
The model learned useful patterns from the training data
Comparing the predicted and actual labels helped me evaluate the model's performance on unseen data.

# Improving Accuracy
What could be done to improve the model's accuracy?
Based on my experiment, increasing the number of hidden layers slightly improved the model's accuracy.

## Model Configuration	Test Accuracy
One hidden layer	0.8917
Two hidden layers	0.8935
This indicates that adding another hidden layer allowed the model to learn additional features from the dataset, resulting in a small improvement in performance.

However, the improvement was minimal, which suggests that simply adding more layers does not always lead to a significant increase in accuracy.


