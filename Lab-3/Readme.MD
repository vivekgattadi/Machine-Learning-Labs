#This is Lab-3!

##Question-1

Develop a Multi-Layer Perceptron (MLP) Neural Network to predict the house prices (Dataset loading function and accessing data matrix and target values have been provided in the code section) Use of built-in library functions for the specific implementation as asked in the questions are not allowed in this section
1. Perform an exploratory analysis on the given dataset. Print the avg, max & min values of each column. Also, show the coorelation of each column with the target values in the dataset using multi-plots. (3 point)

2. Perform data pre-processing operations like standardization and splitting (80:20) of data. (2 points)
3. Implement the three layer fully connected MLP feedforward model with only one hidden layer having 15 hidden units + bias. For this problem make your decision on the number of output units. Also, your implementation should facilitate a choice between Sigmoid & Tanh actionations at each layer of MLP for the user. ( 15 points)
4. Implement Back-propagation algorithm to train the parameters of the MLP created in the previous section. The Backpropagation should support gradient flow for both Sigmoid and Tanh activation functions. (15 points)
5. Train your model using the Mean Sqaured Errors. Mention your choices of the hyperparameters for training. Perform traning with batch gradient descent and stochastic gradeint descent. Plot the graph of traning error versus Epochs for both the training methods. Report the final accuracy you achieved on the Test Data using both the traning methods. (2+3 = 5)
6. Using the best traning method from the above traning, train your MLP with different learning rates given as [ 0.5, 0.1, 0.01, 0.001, 0.0001]. (5 points)
7. Plot the training error versus epochs for each learning rate in a single line graph. Also, plot accuracy versus lerning rate. Comment on your observations. (3+2 = 5 points)


##Question-2

In this question, we will learn to perform multi-class classification on Fashion-MNIST using a convolutional neural network.

1. Explore the Dataset. Display one randomly selected image from each fashion class. (5 points)
2. Plot the distribution of number of images in each fashion class. Is the distribution uniform? Comment. (5 points)
3. Implememnt the 2D convolution function using a kernel size of 3x3. Use the sobel kernel and display the feature map for one example from each fashion class. For using sobel kernel, you need to calculate two convolutions, one for x-direction (x) and one for y-direction (y), the feature map then can be calculated as  𝐹𝑚=(√𝑥2+𝑦2) (10 points)
4. Using the Keras library, implement a CNN model for classification. Use the following network architecture: (5 points)
    - Input layer
    - Con2D with 32 3x3 kernals and ReLU activation
    - Max Pooling layer with pool-size 2x2
    - Con2D with 64 3x3 kernals and ReLU ReLU activation
    - Max Pooling layer with size 2x2
    - Dropout
    -Fully Connected Layer with softmax activation

5. Implement a custom cross-entropy loss (error function) for the multi-class classification. Use it for traning the model. (5 points)
6. Compile and train your model with four different optimizers viz. SGD RMSprop, Adam, Adagrad. Plot the training loss for all four optimizers. Comment on your observations. (10 points)
7. Choose different hyperparameters for Conv Layers, change number of Conv layer and drop-out rate and train your model. Plot training and test accuracies and losses wrt epochs for different hyper-parameters. Do you find any improvement in classification performance. Report your analysis. (10 points)
