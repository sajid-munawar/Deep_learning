**Familiarity with many simple mathematical concepts:**
1. Tensors
2. Tensor operations
3. Differentiation
4. Gradient descent

The core building block of neural networks is the **_layer_**, a data-processing module that
you can think of as a filter for data. Some data goes in, and it comes out in a more useful form. Specifically, layers extract representations out of the data fed into them hopefully, representations that are more meaningful for the problem at hand. Most of
deep learning consists of chaining together simple layers that will implement a form
of progressive data distillation. A deep-learning model is like a sieve for data processing, made of a succession of increasingly refined data filters—the layers.

**Dense layers**, which are densely
connected (also called fully connected) neural layers.

**softmax layer**, which means it will return an array of 10 probability scores (summing to 1)

To make the network ready for training, we need to pick three more things, as part
of the compilation step:
1. A loss function—How the network will be able to measure its performance on
the training data, and thus how it will be able to steer itself in the right direction.
2. An optimizer—The mechanism through which the network will update itself
based on the data it sees and its loss function.
3. Metrics to monitor during training and testing—Here, we’ll only care about accuracy (the fraction of the images that were correctly classified).