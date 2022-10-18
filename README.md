# Variational-Autoencoder

## Introduction

This project implements a Variational Autoencoder (VAE) that takes a hand-written digit as input and encodes it as a multivariate normal distribution where all of the dimensions are independent; Then this distribution is sampled and used to reconstruct the same image. VAEs consist of two main sub-models: the encoder and the decoder. The encoder outputs the estimated distribution of the input image, and The decoder takes the estimated distribution and outputs the reconstructed images. AVEs are unsupervised learning models.

## Data set

I utilized the MNIST database

## References

[LeCun et al., 1998a]
Y. LeCun, L. Bottou, Y. Bengio, and P. Haffner. "Gradient-based learning applied to document recognition." Proceedings of the IEEE, 86(11):2278-2324, November 1998
