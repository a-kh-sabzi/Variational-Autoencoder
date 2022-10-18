# Variational-Autoencoder

## Introduction

This project implements a Variational Autoencoder (VAE) that takes a handwritten digit as input and encodes it as a multivariate normal distribution where all of the dimensions are independent; Then this distribution is sampled and used to reconstruct the same image. 

## Dataset

The MNIST dataset is utilized for training and testing the Variational Autoencoder (VAE) model. This dataset consisits of 60000 and 10000 handwritten digits for training and test sets repectively. The data consists of 10 classes, and Each sample is a 28x28 grayscale image.

![examples from the training set](/assets/images/training_samples.png)

![examples from the test set](/assets/images/test_samples.png)

## Variational-Autoencoder (VAE)

VAEs consist of two main sub-models: the encoder and the decoder. The encoder outputs the estimated distribution of the input image, and The decoder takes the estimated distribution and outputs the reconstructed images. AVEs are unsupervised learning models. It was assumed that the input data can be modoled with a multivariate normal distribution where all of the dimensions are independent; Thus the encoder outputs the means and standard deviations of the estimated distribution. VAEs have many applications such as generating artificial data. After the training is complete, the decoder can be used to generate similar data by receiving noise vectors as input.

## Training

The network was trained on 60000 samples for 10 epoch; The process and other hyperparameters are shown in the accompanying python notebook.  

## Evaluation

The network was evaluated on 10000 new samples.

![examples from the training set](/assets/images/eval_samples_training.png)

![examples from the test set](/assets/images/eval_samples_test.png)

## References

[LeCun et al., 1998a]
Y. LeCun, L. Bottou, Y. Bengio, and P. Haffner. "Gradient-based learning applied to document recognition." Proceedings of the IEEE, 86(11):2278-2324, November 1998.
