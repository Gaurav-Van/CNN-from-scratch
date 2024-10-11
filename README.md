# CNN-from-scratch
Revising concepts of CNN by building them from scratch using NumPy. 
<hr>

## Best Resource for Revision of ANN and CNN 
One of the best playlist for revision of concepts of ANN and CNN. <br><br> https://youtube.com/playlist?list=PLQ4osgQ7WN6PGnvt6tzLAVAEMsL3LBqpm&feature=shared <br><br> The code is taken from this playlist to experiment with, learn, revise, and implement the concept on my own.
<hr>

### File and Class Structure
File `layer.py`: Layer Class providing Blueprint for neural network layers, defining basic attributes for input and output, and placeholder methods for forward and backward propagation. It serves as an interface to be inherited by other classes for specific implementations  

File `activation.py`: The Activation class inherits from Layer and implements activation functions for neural networks. It includes methods for forward propagation using the activation function and backward propagation using the derivative of the activation function.

File `activations.py`: Collection of different activation functions classes. <ins>**Tanh**</ins> Class: The Tanh class inherits from Activation and implements the hyperbolic tangent activation function and its derivative. <ins>**Sigmoid**</ins> Class: The Sigmoid class inherits from Activation and implements the sigmoid activation function and its derivative. <ins>**Softmax**</ins> Class: The Softmax class inherits from Layer and implements the softmax activation function for forward propagation and its gradient for backward propagation.

File `convolutional.py`: The Convolutional class inherits from Layer and implements a convolutional layer for neural networks. It includes methods for forward propagation using 2D convolution and backward propagation to update kernels and biases based on the gradient.

File `dense.py`: The Dense class inherits from Layer and implements a fully connected (dense) layer for neural networks. It includes methods for forward propagation to compute the weighted sum of inputs plus bias, and backward propagation to update weights and biases based on the gradient.

File `losses.py`: Contains functions for calculating loss and its derivatives, which are essential for training neural networks. <ins>**mse**</ins>: Computes the Mean Squared Error (MSE) between the true and predicted values. <ins>**mse_prime**</ins>: Computes the derivative of the MSE loss. <ins>**binary_cross_entropy**</ins>: Computes the Binary Cross-Entropy loss between the true and predicted values. <ins>**binary_cross_entropy_prime**</ins>: Computes the derivative of the Binary Cross-Entropy loss. 

File `network.py`: This file contains functions for predicting outputs and training a neural network. <ins>**predict**</ins>: Takes a network and an input, and returns the output by performing forward propagation through all layers. <ins>**train**</ins>: Trains the network using the specified loss function and its derivative, iterating over the training data for a given number of epochs and updating the network’s weights and biases.

File `reshape.py`: The Reshape class inherits from Layer and implements functionality to reshape the input data into a specified output shape during forward propagation and to revert it back to the original shape during backward propagation.

File `mnist_conv.py`: This file demonstrates how to build, train, and test a convolutional neural network on the MNIST dataset using custom layers and activation functions. **Data Preprocessing**: The <ins>preprocess_data</ins> function prepares the MNIST data by normalizing and reshaping it. **Network Definition**: The network consists of convolutional, reshape, and dense layers with sigmoid activations. **Training**: The <ins>train</ins> function trains the network using binary cross-entropy loss. **Testing**: The network’s performance is evaluated on the test set, printing predicted and true labels.
<hr>

### Key Concepts from Playlist Videos
![image](https://github.com/user-attachments/assets/81bbba05-18ef-453f-8c70-adf63aa28421)

`2 Types of Operations - valid and full`<br><br>`valid`<br>
![image](https://github.com/user-attachments/assets/4cf65004-7e26-478e-8dac-8dbb2aa2bf95)
`full`<br>
![image](https://github.com/user-attachments/assets/2d8d1fbe-4bf4-4b85-b758-e9c0a96574dd)

`Forward Propagation`
![image](https://github.com/user-attachments/assets/9a1a791d-51e1-4fc4-ad32-71167314299e)

`Backward Propagation`: Reason of taking derivate of error with respect to input in backpropagation. We are essentially looking at how the output of previous layer effects the error. Because the input of current layer is the output from the previous layer. 
![image](https://github.com/user-attachments/assets/25154427-5b97-4610-af45-041e654b640d)
![image](https://github.com/user-attachments/assets/f6c5f66c-5c6d-4d2c-a058-e76698ee262b)

