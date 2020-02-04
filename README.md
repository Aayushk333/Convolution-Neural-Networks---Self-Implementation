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

<caption><center> <u> <font color='purple'> **Figure 2** </u><font color='purple'>  : **Convolution operation**<br> with a filter of 3x3 and a stride of 1 (stride = amount you move the window each time you slide) </center></caption>

Each value in the matrix on the left corresponds to a single pixel value, and we convolve a 3x3 filter with the image by multiplying its values element-wise with the original matrix, then summing them up and adding a bias. 


## 4 - Pooling layer 

The pooling (POOL) layer reduces the height and width of the input. It helps reduce computation, as well as helps make feature detectors more invariant to its position in the input. The two types of pooling layers are: 

- Max-pooling layer: slides an ($f, f$) window over the input and stores the max value of the window in the output.

- Average-pooling layer: slides an ($f, f$) window over the input and stores the average value of the window in the output.

