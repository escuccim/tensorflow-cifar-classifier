# TensorFlow CIFAR classifier

A classifier for CIFAR10 data written in TensorFlow.

The model is a 6-layer convolutional neural network structured as follows:

1. Convolutional Layer 1 - 32 3x3 units (no activation)
2. Batch Normalization
3. Relu activation
2. Convolutional Layer 2 - 32 3x3 units (no activation)
4. Batch normalization
5. Relu activation
3. 2x2 Max Pooling Layer
4. Dropout at 25%
5. Convolutional Layer 3 - 64 3x3 units (Relu activation)
6. Convolutional Layer 4 - 64 3x3 units (no activation)
8. Batch normalization
9. Relu activation
7. 3x3 Max Pooling Layer
8. Dropout at 25%
9. Flatten output
10. Fully connected layer with 512 units and Relu activation
11. Dropout at 50%
12. Logits

The model is created in TensorFlow and includes logging hooks for TensorBoard. I am in the process of training the data with the CIFAR10-50k data set.

The model is currently in a Jupyter notebook. I plan on converting it to .py files after it has been trained.
