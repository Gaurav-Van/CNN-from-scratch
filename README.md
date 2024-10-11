# CNN-from-scratch
Revising concepts of CNN by building them from scratch using NumPy. 
<hr>

## Best Resource for Revision of ANN and CNN 
One of the best playlist for revision of concepts of ANN and CNN. <br><br> https://youtube.com/playlist?list=PLQ4osgQ7WN6PGnvt6tzLAVAEMsL3LBqpm&feature=shared <br><br> The code is taken from this playlist to experiment with, learn, revise, and implement the concept on my own.
<hr>

### Class Structure
Class `layer`: Class providing Blueprint for neural network layers, defining basic attributes for input and output, and placeholder methods for forward and backward propagation. It serves as an interface to be inherited by other classes for specific implementations  

Class ``

<hr>

### Important Concepts from playlist videos 
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

