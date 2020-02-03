# Convolution-Neural-Networks---Self-Implementation

## Outline of the Project

We will be implementing the building blocks of a convolutional neural network! Each function we will implement will have detailed instructions.

- Convolution functions, including:
    - Zero Padding
    - Convolve window 
    - Convolution forward
- Pooling functions, including:
    - Pooling forward
    - Create mask 
    - Distribute value
    
    This following is the architecture of a basic Convolutional Neural Network model. We will be implementing basic building 
    blocks required to build this model from scratch. 
    
    <img src="architecture.png" style="width:800px;height:300px;">


### Single step of convolution 

In this part, we implement a single step of convolution, in which we apply the filter to a single position of the input. This will be used to build a convolutional unit, which: 

- Takes an input volume 
- Applies a filter at every position of the input
- Outputs another volume (usually of different size)

    <img src="Convolution operation.gif" style="width:500px;height:300px;">
