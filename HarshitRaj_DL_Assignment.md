# Nueral Networks
**Neural Network** is one of the significant algorithms to understand **DEEP LEARNING**. This method is base on the neural networks working in a **human brain**.
This algorithm solved many unsolvable problems in the field of **Artificial Intelligence**.
It was first introduced in  1943. The same year deep learning was introduced. We can say that the deep learning brain works on Neural Network Algorithm.

## What is NEURAL NETWORK
It has only three-layer 
1. Input Layer
2. hidden Layer
3. Output Layer

The **input layer** takes in the data feature. The **hidden layer** handles the calculation of ***weights*** according to the feature given for the input layer. Then the **output layer** gives out the result based on the calculation of the hidden layer.
There will be only one Input Layer and one Output Layer, but the hidden layer can consist of multiple layers based on the problems' complexity.
For example, a very famous model is used for image recognition called **VGG-16(Visual Geometry Group-16)** the no. Sixteen in this represent the layers present in this particular neural network.
There are 16 layers in this in which there is **one input layer** and **one output layer** and **14 hidden layers**.
All the layers consist of nodes and those noes holds the value after calculation
### INPUT LAYER
The input layer is starting layer of nueral layer. It takes the input from the data base (data feature is the actuall input) and then the processing of the that input is done in further layers. 
The no. of features decide the no. of nodes in the input layer 
For example if there are **F** no. of feature then there will be **F** no. of nodes in input layers.
In **FIG 1** there are 3 nodes in input layer so the input layer will take three features of the data as input.
In  this layer there will be no activation function and no normalzation of data not performed. Dta normalization is done before the input layer.
### HIDDEN LAYER
This layer is the internal layer and the main layer, every computation of the weights and proceesing of data features are also done here.
In this layer no. of nodes are optional to keep but it is recomended that if model should perform better we should use the equal no. of nodes as in input layer or more than that.
For example, if there are **n** nodes in input layer then there should be n nodes or more than n node in hidden layer.
Hidden layer is itself combination of multiple layer as you can see in **FIG 1** there are 2 layers in hidden layer.
In this layer every sub layer will have an extra node for the bias.
Every node in this layer will have an **activation function**. **Sigmoid** and **Relu** are the most commonly used activation function. These fucntion keep the value of the node and weights in a particular range.
#### Sigmoid Function
![Sigmoid FUnction](https://analyticsindiamag.com/wp-content/uploads/2018/01/sigmoid-equation.png)

**FIG SIGMOIF FUNC**

This function usually keep the value from 0 to 1. If the value of **x ** is **negetive** then the value of **f(x)** will be **nearer to zero** and if the value of **x** is **possitive** then the value of **f(x)** will be **nearer to 1** and if the value of **x** is **zero** then the value of **f(x) is zero**.
***NOte:- Here x is not the input value from the input layer instead it is the value of the node*** 

#### ReLu Function
![ReLu Function](https://i0.wp.com/highontechs.com/wp-content/uploads/2020/06/activation-functions3-3.jpg?resize=351%2C232&ssl=1)

![Nueral Netwokk image](https://icdn.digitaltrends.com/image/digitaltrends/artificial_neural_network_1-327x238.jpg)


**FIG 1**

## Weights
These weights are significant of the neural networks. This helps the NN to calculate the output of the data feature. 
![formaulae Image](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/02/Screenshot-from-2020-02-03-22-14-21.png)

**FIG 2**

Here the w represents the weights, X is the input from the prev layer, and b is the bias. 
Initially, the weights are initialized to random value but not zero (since the value is getting multiplied).
Deep Learning is considered the successor of machine Leaning. So MAchine learning is basically a training model to get perfect results matching the labelled diagram.
So what it is that we train actually in the model? It is the weight of what we train.
As we can see that the formulae in **FIG 2** (the first line). 
W is the weight that gets updated simultaneously while training. 
When we get the perfect weights, we stop training the model, and we get the final full trained model. 
Now the big questions are which weights should be selected?
The weights which give the prediction and accuracy value high, then we can say that the weights are perfect for that value.

### What are Weights.
As we can see in **FIG 1** the nodes are comnected with the lines that means while training the value psses throught he nodes using these lines.
These lines are only considered as the weights. The wieghts are bascally represented as the matrix. The dimension of the matrix is (n * m) where n represents the no. of nodes on the left side (previous layer) and m represents the no. of nodes presents in right side (next layer). 
I fyou see in **FIG 1** the weights between hidden layer 1 and hidden layer 2 will be of matrix (no. of nodes in hidden layer 2 * no. of nodes in hidden layer 1) i.e  4*4.

It is essential to do matrix multiplication, as we can see in **FIG 2**, because we do not get only one feature of data in real-world problems.
We need multiple nodes in the input layer for multiple features and then compute the output correctly; we need to use the same or more no. of nodes in every hidden layer.



