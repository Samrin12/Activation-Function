# Activation-Function
Activation functions are essential components of neural networks, serving a critical role in hidden layers to address complex problems and to process and convey input throughout deep learning algorithms. Activation functions execute non-linear calculations. The functions in a neural network calculate the weighted total of inputs and biases to determine if a neuron can be triggered. The activation function's primary role is to convert the combined weighted input from a node into an output value that is then forwarded to the next hidden layer or utilized as the final output according to the following figure. 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/d5b34068-270f-4858-a925-6fece5ef03ba)

Each neuron in a neural network performs two computations.
The diagram shows the linear combination of two inputs, x1 and x2, with corresponding weights w1 and w2, and a bias b. The formula represents the linear sum.

z = w1x1 + w2x2 + ... + wnxn +b

This calculation determines if a neuron should be triggered based on the weighted sum and an additional bias. The activation function's role is to bring non-linearity to the neuron's output. If the value is above the activation function's threshold, it will activate; otherwise, it will generate a very small value for values below the threshold. The following figure demonstrates the architecture of a neural network. 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/2947a7a4-191d-497e-98fa-c1c71f052a26)

It is utilized in a neural network to determine the outcome of a neural network, such as a binary decision between "yes" or "no." The values are mapped to a range of 0 to 1 or -1 to 1 based on the function. Activation functions are the following types. They are:
1.	Binary Step Function.
2.	Linear Activation Function.
3.	Non-linear Activation Function.

### Binary Step Function: 
The binary step function acts as a gate that operates only when a particular threshold value is reached. When the input exceeds the threshold, the neuron becomes activated; otherwise, it remains inactive. Once a neuron is triggered, the output from the previous layer is transmitted to the subsequent level of the neural network's hidden layers. The binary step function operates based on a fixed threshold and has disadvantages, including a lack of differentiability and an inability to backpropagate signals. The equation and graphical representation of the binary step function are given below. 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/376c09db-da4e-45f9-ba07-1c6fc739ed81)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/4c433be5-8d54-45da-958a-c5a3aa18b2fc)

### Linear Activation Function:
The linear activation functions, sometimes referred to as identity functions, are mainly used to maintain the output equivalent to the input signal. The identity function is non-derivative and does not alter the signal going through it, making it unsuitable for use in the innermost layers of a deep learning network. The equation and graphical representation of the linear activation function are given below. 
F(x) = x

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/7349f785-bb5a-4d88-ad96-d01a3b0325c2)

### Non-Linear Activation Function: 
Nonlinear activation functions are the most often utilized in neural networks. Non-linear activation functions offer benefits by aiding in backpropagation and enabling stacking. Non-linear combinations of functions inside a network facilitate the development and training of a model capable of adjusting weights and biases, with outputs represented as a functional computation. Non-linear activation functions enhance the measurement of inputs, outputs, and processes inside a neural network, leading to adjustments in equations until desired outputs are obtained. Activation functions enable back-propagation by providing gradients that are used to adjust the weights and biases based on the mistake. Key terms essential for understanding nonlinear functions include:

**Differential or derivatives:** Change in the y-axis relative to the change in the x-axis. It is commonly referred to as a slope.

**Monotonic function:** A function that is strictly increasing or decreasing.

The non-linear activation Functions are primarily categorized based on their range or curve. The basic types of nonlinear functions, their equations, and graphic representations are given below. 

**1.Sigmoid Function:** This function accepts any real number as an input and produces output numbers within the range of 0 to 1. As the input increases, the output value approaches 1, and as the input decreases, the output approaches 0. The equation and the graphical representation of the function are, 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/4df34ab3-538b-42c8-ad26-552c56e232cd)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/4e38803f-73d3-4a39-87a4-b567796dd76e)

**2.Hyperbolic Tangent Function (tanh):** The Tanh function closely resembles the sigmoid/logistic activation function, both exhibiting an S-shape, with the distinction being the output range of -1 to 1. As the input in Tanh increases, the output approaches 1, and as the input decreases, the output approaches -1. The equation and the graphical representation of the function are, 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/e24048de-c6e6-4699-aba1-339dca036cfe)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/1fa2dfc9-cf6c-4b99-a100-57ddd5f88717)


**3.Rectified Linear Unit (ReLU):** Not all input values will trigger the ReLU function. Activation will occur only if the input value exceeds 0. The equation and graphical representation of the ReLU function are, 

F(x) = x, if x> 0

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/d33c35b5-9ef0-4a27-bb88-002923b117c9)

**4.Leaky ReLU:** Leaky ReLU is an enhanced version of the ReLU function designed to address the issue of the Dying ReLU problem by introducing a slight positive slope in the negative region. The equation and graphical representation of the Leaky ReLU function are, 

F(x) = (0.1x, x)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/5ebf51f8-1f01-42b3-b06f-004cab9eb3b0)

**5.Exponential Linear Unit (ELU):** ELU, short for Exponential Linear Unit, is a variation of ReLU that adjusts the slope of the negative segment of the function. ELU utilizes a logarithmic curve to represent negative values, unlike the leaky ReLU and Parametric ReLU functions, which use a linear line. The equation and graphical representation of the ELU function are, 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/bb0a2b0c-b8c8-4a68-a2be-6caf85e344a6)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/63b8d096-8022-4255-b0f7-6d1dd1e0ed16)


**6.Scaled Exponential Linear Unit (SELU):** Scaled Exponential Linear Units, also known as SELUs, are activation functions that have the ability to provide self-normalizing characteristics. The equation and graphical representation of the SELU function are, 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/42410ac6-d29c-4efd-b6b6-98f57bb939d8)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/95fbef91-5447-43dd-8f00-cd22c7d2986e)

**7.Softmax Function:** The softmax function is used in the output layer for problems involving multi-class categorization. It converts original values into probabilities, guaranteeing that the total probability for all classes equals 1. The equation and graphical representation of the Softmax function are,

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/ae370db3-cbbb-4c5f-af1e-4bc8ba19b803)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/3f9a3b0e-753c-439b-8eb0-30c93eadd79e)

**8.Swish Function:** Swish function is a self-gated activation function. Swish routinely equals or surpasses the ReLU activation function in deep networks used for tasks like image classification and machine translation. The function and graphical representation of the swish function are,

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/27a83e1a-a1bf-43d3-af21-0305e9fd449a)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/8361c532-5ace-41a6-a857-00cc9d5ee185)


## Analysis of the Activation Functions and Implementation of Sigmoid and ReLU Activation Functions: 
The sigmoid function is effective in output layers for classification problems because of its smooth and restricted output range of 0 to 1, matching probabilities. However, its high processing cost and tendency for gradients to vanish limit its applicability in hidden layers. ReLU is particularly effective in hidden layers of deep networks because of its quick computation, effectiveness, and ability to prevent vanishing gradients. It excels in regression tasks with possibly infinite results. Nevertheless, it can result in the death of neurons and necessitates cautious management. Leaky ReLU can be utilized to overcome the restrictions of ReLU, tanh can provide a similar output range to Sigmoid but with quicker computation, and Swish is known for its smooth non-linear properties.

This work includes the implementation of the widely used Sigmoid and ReLU activation functions. The following code was written to generate the sigmoid activation function and ReLU activation function respectively.

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/73202c86-4420-41b2-b4e5-e7605ea56fd2)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/e290ab6f-a7a7-44d5-b24e-717ac666fa8f)

I have set random continuous values within a specified range as default input values. The code also allows users to enter values on their own. The subsequent code will produce a prompt that let the user to choose whether they want to execute the function using the default value or whether they intend to provide the input according to their preference.

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/32a7ed20-3e53-4529-983c-c0a77b616a00)

The resultant output of the code is, 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/6940ffa6-6325-4f21-a0ec-fd3a45a7f01a)

The output graph for the sigmoid function and the ReLU function for a given continuous value from the range of -10 to 10 with a step value of 0.2 are given below. 

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/6dfad6e7-d266-4679-80e6-4331c8e8e35c)

![image](https://github.com/Samrin12/Activation-Function/assets/87581935/5fee4b71-2314-4047-b192-69fc96e9a581)











