# What Gradient Descent Algorithm used for?
Gradient descent is the optimizer that we used to minimize the loss function or we can say error value which helps in improving the model performance and accuracy.

# What is loss function?
Loss function here is the mistakes or error that our model is making during prediction or classification, so to reduce that error in our model we use gradient descent algorithm which optimizes our model output.

## Before getting the understanding of how GD algorithm works and its implementation lets understand the concept of weights.
![image](https://github.com/shresth-H/Deep-Learning/assets/57328884/ea6e0e4b-e024-4c93-952a-d488096e9ec9)
This is the simple representation of the single node in neural network consists of input nodes representing features in the model.

![image](https://github.com/shresth-H/Deep-Learning/assets/57328884/ae3fc5e6-2ca7-4e48-b36a-f9e8f4682780)
Now before training of model begins we assign some random weights to these input nodes, and the weight parameter here tells us the importance of that node or feature in the model output. We calculate the submission of the input values multiplied by weight paramter and then the result achieved will passed throught the activation function to produce an output for each node in the layer.

This process repeats for all the nodes in hidden layer until the final output of the model is generated.

Now this result is the predcited value of the neural network which is been compared to the actual value and finally by finding the different between the actual value and the predicted value we get to know the error value of our model.
To increase the accurracy of our model we need to minimize the error value which we achieve by modifying this weight parameter using gradient descent algorithm.


## Lets understand some mathematical aspects that you should be aware of

### what is local and global Minima value of the funtion
The point at which the function takes the minimum value is the global minima and the local minima are the point from where we have continuous increament in value of a function.

Global minima and All local Minima values are defined where the first derivative of the function is zero.
Derivative is the differentiation of the function which is d/dx of f(x)

# How GDA works?
![image](https://github.com/shresth-H/Deep-Learning/assets/57328884/6eee5f0f-1169-4f46-9572-dc49c953c473)

As represented in this graph we have a weight on x axis and loss function on y axis, first step is to assign random guesss for weight parameter, so when we use initial weight to calculate loss function values it gives error value of our model output.

Now to reduce this error we will modify our weight parameter until our weight value reaches to the global minima which is global cost minimum here, at global minima we have the minimum error value for loss function where the model predicts the value with maximum accuracy.

The formula to modify the weight paramter:  GM1 = GM0 - α∇f(X0​)

minima is a initial weight 
Gradient is the differentitaion of the loss function and the
Learning rate is the step size in the direction of required weight or global minima. ( It also tells us how fast or slow our model is learning. if we use small learning rate the algorithm may take a long time to get to the global minima and if we use large leaning rate the algorithm might miss the global minima and oscillates around it )
The iterations use to update the weight parameter are the training epochs.


