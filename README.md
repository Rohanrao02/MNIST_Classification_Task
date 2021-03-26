# MNIST_Classification_Task


According to the problem statement, the task was to classify the images of handwritten digits using deep Neural Networks. The dataset used was downloaded from Kaggle. It consists of 60,000 examples in train set ad 10,000 in test set. Each image was of size 28 x 28.
Inspiration for my code was mostly drawn from the materials taught in Deep Learning Specialization course by DeepLearning.AI and from official TensorFlow website.

For the classification problem using deep Neural network, most of the codes were written from scratch. The data obtained was separated into labels and images and then normalized. Parameters were initialized using ‘He’ initialization and Softmax loss (Categorical Cross Entropy loss) was used to calculate cost function (Multi Class Classification). Optimization was done using ‘Adam’ optimization method.
For cross validation of data, the whole training set was used because after using 1000 training examples for each mini batch, the training set gets reduced to 60 mini batches. Tuning of various hyper parameters have been shown in the code.
Final test accuracy obtained is 97.71%

Bonus Problem Statement 1:
Here, the task was to classify the images of hand written digits using a Convolutional Neural Network.
The architecture used is similar to LeNet – 5. LeNet – 5 takes input images of size 32 x 32. As my input image is of size 28 x 28, I have used ‘same’ convolution instead of valid convolution with 5 x 5 filters. Rest of layers used are similar to that of LeNet-5 architecture.
The model was created using TensorFlow framework. CNN learns the filters automatically without mentioning explicitly. Filters help in extracting right and relevant features from input image and captures spatial features.
Final test accuracy obtained is 98.27%

Bonus Problem Statement 2:
The task here is to create a model which detects square number among the label. Hence the problem becomes a simple Binary classification task.
So, the modification includes change in the labels of dataset to either 1 or 0 based on whether the number is either square number or not. Other changes include change in cost function and activation of output layer. Binary Cross entropy is used to calculate cost function and Sigmoid function is used as the activation of output layer instead of Softmax activation.
Final test accuracy is 98.17%
