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
