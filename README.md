# TensorFlow CIFAR classifier

A classifier for CIFAR10 data written in TensorFlow.

In the jupyter notebook I create, train and compare five models for classifying the CIFAR10 data.

## Model 1 Architecture

1. Conv 1
    1. 64 5x5 units with a stride of 1
    2. Batch normalization
    3. Relu activation
2. Max Pool 1 size 3x3 with stride 2
    1. Dropout at .125
3. Conv 2
    1. 64 5x5 units with a stride of 1
    2. Batch normalization
    3. Relu activation
4. Max Pool 2 size 3x3 with stride 2
    1. Dropout at 0.125
5. Flatten output
    1. Dropout at 0.25
6. Fully connected layer 1 with 384 units
    1. Batch normalization
    2. Relu activation
7. Fully connected layer 2 with 192 units
    1. Dropout at 0.25
8. Logits

## Model 2 Architecture

1. Conv 1
    1. 32 3x3 units with a stride of 2
    2. Batch normalization
    3. Relu activation
2. Conv 2
    1. 32 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
3. Max Pool 1 2x2 with stride of 1
    1. Dropout at 0.125
4. Conv 3
    1. 64 3x3 units with stride of 2
    2. Batch normalization
    3. Relu activation
5. Conv 4
    1. 64 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
6. Max Pool 2 3x3 with stride of 2
    1. Dropout at 0.125
7. Flatten output
    1. Dropout at 0.125
8. Fully connected layer 1
    1. 512 units with relu activation
    2. Dropout at 0.25
9. Logits

## Model 3 Architecture

1. Conv 1
    1. 32 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
2. Conv 2
    1. 32 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
3. Max Pool 1 2x2 with stride of 2
    1. Dropout at 0.1
4. Conv 3
    1. 64 3x3 units with stride of 1
    2. Batch normalization
    3. Relu activation
    4. Dropout at 0.1
5. Conv 4
    1. 64 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
6. Max Pool 2 2x2 with stride of 2
7. Conv 5
    1. 128 3x3 units with stride of 1
    2. Relu activation
    3. Dropout at 0.1
8. Conv 6
    1. 128 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
9. Max Pool 3 2x2 with stride of 2
10. Flatten output
    1. Dropout at 0.1
11. Fully connected layer 1
    1. 1024 units with relu activation
    2. Dropout at 0.1
12. Logits

## Model 4 Architecture

1. Conv 1
    1. 32 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
2. Conv 2
    1. 32 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
3. Max Pool 1 2x2 with stride of 1
    1. Dropout at 0.125
4. Conv 3
    1. 64 3x3 units with stride of 1
    2. Batch normalization
    3. Relu activation
5. Conv 4
    1. 64 3x3 units with a stride of 1
    2. Batch normalization
    3. Relu activation
6. Max Pool 2 3x3 with stride of 2
    1. Dropout at 0.125
8. Fully connected layer 1
    1. 512 units with relu activation
    2. Dropout at 0.25
9. Logits
