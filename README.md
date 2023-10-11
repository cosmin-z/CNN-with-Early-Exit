# CNN with Early exit

This Repository refers to the Final Project of the course [Neural Networks for Data Science (NNDS)](https://www.sscardapane.it/teaching/nnds-2022/) at University Sapienza of Rome 2022/2023.

## Abstract

## Dataset

The dataset chosen for this homework is [**Cards Image**](https://www.kaggle.com/datasets/gpiosenka/cards-image-datasetclassification) from kaggle. It consist of 7624 training images, 265 test images and 265 validation images with 53 different categories (a 'normal' French deck, look at the joker card into the test set). Each image is an rgb image and the particularity of these cards is that they are all very different from each other both in design and with respect to contrasts.


The idea of using this dataset is because usually the neural network try to predict values in small range in this case we have 53 different categories.

The task is Image Classification.

Since my dataset is not stored separately in train/validation/test i did it myself. I divided the data as follows:

*   70% train set
*   15% validation set
*   15% test set

## First Model : CNN

I decided to use a convolutional neural network with 4 convolutional blocks of different sizes, a flattening layer and a classification block. Each convolutional block is composed by:

*Convolutional layer
*Batch Normalization
*ReLu
Max Polooing 2D

In addition I've included some regularization.
