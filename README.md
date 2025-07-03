# MNIST_classification-using-ANN
 Handwritten Digit Recognition using Neural Networks
This project demonstrates a basic implementation of a neural network using TensorFlow and Keras to recognize handwritten digits from the MNIST dataset.

-> Dataset
We use the MNIST dataset, which consists of:
60,000 training images
10,000 testing images
Each image is a 28x28 grayscale image of a digit from 0 to 9.

-> Project Structure
Data Preprocessing:
Loaded MNIST dataset using keras.datasets.mnist.
Normalized pixel values to the range [0, 1] by dividing by 255.

-> Model Architecture:
Flatten layer to convert 2D images into 1D vectors.
Dense hidden layer with 128 neurons and ReLU activation.
Output layer with 10 neurons (for digits 0–9) using Softmax activation.

-> Compilation & Training:
Optimizer: adam
Loss function: sparse_categorical_crossentropy
Evaluation metric: accuracy
Trained for 10 epochs with 20% validation split.

-> Model Evaluation
Used model.predict() to get probabilities.
Converted probabilities to class predictions using argmax.
Evaluated accuracy using sklearn.metrics.accuracy_score.

-> Performance Visualization
Loss and accuracy trends across epochs are plotted using matplotlib.
