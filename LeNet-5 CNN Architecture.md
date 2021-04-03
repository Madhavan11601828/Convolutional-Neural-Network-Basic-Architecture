# LeNet-5 Architecture

In 1998, the LeNet-5 architecture was introduced in a research paper titled [Gradient-Based Learning Applied to Document Recognition” by Yann LeCun, Leon Bottou, Yoshua Bengio, and Patrick Haffner](https://ieeexplore.ieee.org/abstract/document/726791). It is one of the earliest and most basic CNN architecture.

It consists of 7 layers. The first layer consists of an input image with dimensions of 32×32. It is convolved with 6 filters of size 5×5 resulting in dimension of 28x28x6. The second layer is a Pooling operation which filter size 2×2 and stride of 2. Hence the resulting image dimension will be 14x14x6.

Similarly, the third layer also involves in a convolution operation with 16 filters of size 5×5 followed by a fourth pooling layer with similar filter size of 2×2 and stride of 2. Thus, the resulting image dimension will be reduced to 5x5x16.

Once the image dimension is reduced, the fifth layer is a fully connected convolutional layer with 120 filters each of size 5×5. In this layer, each of the 120 units in this layer will be connected to the 400 (5x5x16) units from the previous layers. The sixth layer is also a fully connected layer with 84 units.

The final seventh layer will be a softmax output layer with ‘n’ possible classes depending upon the number of classes in the dataset.

[LeNet-5 Architecture]()
