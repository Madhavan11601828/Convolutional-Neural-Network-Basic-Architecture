# LeNet-5 Architecture

In 1998, the LeNet-5 architecture was introduced in a research paper titled [Gradient-Based Learning Applied to Document Recognition” by Yann LeCun, Leon Bottou, Yoshua Bengio, and Patrick Haffner](https://ieeexplore.ieee.org/abstract/document/726791). It is one of the earliest and most basic CNN architecture.

It consists of 7 layers. The first layer consists of an input image with dimensions of 32×32. It is convolved with 6 filters of size 5×5 resulting in dimension of 28x28x6. The second layer is a Pooling operation which filter size 2×2 and stride of 2. Hence the resulting image dimension will be 14x14x6.

Similarly, the third layer also involves in a convolution operation with 16 filters of size 5×5 followed by a fourth pooling layer with similar filter size of 2×2 and stride of 2. Thus, the resulting image dimension will be reduced to 5x5x16.

Once the image dimension is reduced, the fifth layer is a fully connected convolutional layer with 120 filters each of size 5×5. In this layer, each of the 120 units in this layer will be connected to the 400 (5x5x16) units from the previous layers. The sixth layer is also a fully connected layer with 84 units.

The final seventh layer will be a softmax output layer with ‘n’ possible classes depending upon the number of classes in the dataset.

In Python Programming, the model type that is most commonly used is the Sequential type. It is the easiest way to build a CNN model in keras. It permits us to build a model layer by layer. The ‘add()’ function is used to add layers to the model. As explained above, for the LeNet-5 architecture, there are two Convolution and Pooling pairs followed by a Flatten layer which is usually used as a connection between Convolution and the Dense layers.

The Dense layers are the ones that are mostly used for the output layers. The activation used is the ‘Softmax’ which gives a probability for each class and they sum up totally to 1. The model will make it’s prediction based on the class with highest probability.

The summary of the model is displayed as below.

[LeNet-5 Architecture](https://github.com/Madhavan11601828/Convolutional-Neural-Network-Basic-Architecture/blob/main/LeNet-5Architectures.PNG)

[Resource](https://www.upgrad.com/blog/basic-cnn-architecture/)
[Resource](https://medium.com/datadriveninvestor/five-powerful-cnn-architectures-b939c9ddd57b target=”_blank” rel=”nofollow”)
[Resource](ttps://medium.com/techiepedia/binary-image-classifier-cnn-using-tensorflow-a3f5d6746697 target=”_blank” rel=”nofollow”)
[Python Programming Model](https://github.com/Madhavan11601828/Convolutional-Neural-Network-Basic-Architecture/blob/main/LeNet-5PythonProgrammingModel.PNG)
