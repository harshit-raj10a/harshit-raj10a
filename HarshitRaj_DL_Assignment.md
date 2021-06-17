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
FIG SIGMOIF FUNCTION

This function usually keep the value from 0 to 1. If the value of **x ** is **negetive** then the value of **f(x)** will be **nearer to zero** and if the value of **x** is       **possitive** then the value of **f(x)** will be **nearer to 1** and if the value of **x** is **zero** then the value of **f(x) is zero**.
***Note:- Here x is not the input value from the input layer instead it is the value of the node***

#### ReLu Function
![ReLu Function](https://i0.wp.com/highontechs.com/wp-content/uploads/2020/06/activation-functions3-3.jpg?resize=351%2C232&ssl=1)
FIG ReLu FUNCTION

This function uses the max function. In this the **negetive** values of **x** is equalized to 0 where as **x** value is the same as it is. The negetive value will always decrese the vaue of fyrther weights and also the values of next layers nodes.
***Note:- Here x is not the input value from the input layer instead it is the value of the node***

#### SOFTMAX FUNCTION
This fumction convert the value of the nodes into the probablity with respect to the sum of the value of all the nodes in the layer.
For exam a layer have 5 nodes whith value 12, 34, 52, 43, 28. After applying softmax function to ecah node the value will be 
Node_1:-12/(12+34+52+43+28)==0.071 * 100==7.1%
Node_2:-34/(12+34+52+43+28)==0.201 * 100==20.1%
Node_3:-52/(12+34+52+43+28)==0.307 * 100==30.7%
Node_4:-43/(12+34+52+43+28)==0.254 * 100==25.4%
Node_5:-28/(12+34+52+43+28)==0.165 * 100==16.5%
sum==                                     99.8
this all values will add up to be 100 or near to it.

### OUTPUT LAYER
This layer is the last layer of the model. It gives out the output what the model has predicted. This layer also have activation fucntion but the activation layer is based on the no. of nodes in output layer. 
For example if the model is classifying only two object like dog vs cat model. SO the model will either detect cat or dog. This is called as binary classification (0 and 1).
This model will have only two nodes in output layer. 
For this this the ***SIGMOID FUNCTION*** is used as the ***activation function***. If the data feature is representing cat and the model classifying correctly it as a cat the then the first node will have the highest possitive value and another will have lowest possitive value or it'll be equal to zero.
When we are using a model which have to classify multiple classes then we have to use ***SOFTMAX FUNCTION*** as the activation function for every node in output layer.
For example if the model is classifying cat, dog, pig, cow and crow. Then the ***softmax function*** wil be used as ***activation fucntion*** for each node of output layer.
This function will increase the value of one node and decrese the value of rest of the node. If the input data feature is labelled as ***pig*** aand the model is clasifyin it correct then the ***node value*** of ***pig*** is ***increased*** and rest all node value is decreased. The node with the highest value is the oupu.


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
We need multiple nodes in the input layer for multiple features.
In the **FIG 2** the Z represents the value of nodes in the next hidden layer.
So now lets examine the matrix mutiplication.
**Z=W(t)X+b.**
The dimension of ***W*** is 4 * 2 (4 rows and 2 collumns) and dimension of ***W(t)*** is 2 * 4 (2 rows and 4 collumns).
As we have discussed above the dimension of W is ( (n * m) where n represents the no. of nodes on the left side (previous layer) and m represents the no. of nodes presents in right side (next layer)) and in ***FIG 2*** the no. of nodes of X is 4 and the no. of nodes in next layer is 2( we can derive this from the dimension of the weights).
and the bias is also of the same shape of ***Z*** since it's getting added to the ***Z*** matrix.
And after the multiplication matrix we get the final value of the ***Z*** matrix. Here the shape of ***Z Matrix*** is 2 * 1 that means there are 2 nodes in the next layer for which we are calculating the node values.
Now, if the next layer is another hidden layer then we have to apply sigmoid or relu function on the node values or on the values of Z matrix and it sholud be applied element wise.
But if the next layer is the output layer then the activation layer should be used based on the model classyfier as discussed above. Here also the activation function should be applied element wise.
