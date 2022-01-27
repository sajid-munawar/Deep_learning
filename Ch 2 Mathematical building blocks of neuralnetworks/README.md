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

**accuracy** (the fraction of the images that were correctly classified).

To make the network ready for training, we need to pick three more things, as part
of the compilation step:
1. A **loss function**—How the network will be able to measure its performance on
the training data, and thus how it will be able to steer itself in the right direction.
2. An **optimizer**—The mechanism through which the network will update itself
based on the data it sees and its loss function.
3. **Metrics** to monitor during training and testing—Here, we’ll only care about accuracy (the fraction of the images that were correctly classified).

**Tensors**

Data stored in multidimensional Numpy
arrays, also called tensors.

**So what’s a tensor?**

At its core, a tensor is a container for data—almost always numerical data. So, it’s a
container for numbers. You may be already familiar with matrices, which are 2D tensors: tensors are a generalization of matrices to an arbitrary number of dimensions
(note that in the context of tensors, a dimension is often called an axis)

 **Scalars (0D tensors)**

A tensor that contains only one number is called a scalar (or scalar tensor, or 0-dimensional
tensor, or 0D tensor). In Numpy, a float32 or float64 number is a scalar tensor (or scalar
array).

 **Vectors (1D tensors)**

An array of numbers is called a vector, or 1D tensor. A 1D tensor is said to have exactly
one axis. 

 **Matrices (2D tensors)**

An array of vectors is a matrix, or 2D tensor. A matrix has two axes (often referred to
rows and columns).

 **Key attributes**

A tensor is defined by three key attributes:
1.  **Number of axes (rank)**—For instance, a 3D tensor has three axes, and a matrix has
two axes. This is also called the tensor’s ndim in Python libraries such as Numpy.
2. **Shape**—This is a tuple of integers that describes how many dimensions the tensor has along each axis.
3.  **Data type** (usually called dtype in Python libraries)—This is the type of the data
contained in the tensor