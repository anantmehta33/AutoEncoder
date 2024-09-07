# Autoencoder-Based Project

This project implements an autoencoder neural network for dimensionality reduction and data reconstruction. Autoencoders are unsupervised learning models designed to learn efficient encodings of input data and reconstruct the input from these encodings. The primary objective of this project is to demonstrate how autoencoders can compress data and then reconstruct it with minimal loss.

## Table of Contents
- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Autoencoder Overview](#autoencoder-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Autoencoders are neural networks designed to replicate their input by learning a compressed representation of data, known as the bottleneck layer. In this project, we build an autoencoder using PyTorch to compress images and then reconstruct them from their compressed form.

The autoencoder is trained using the MNIST dataset, which contains 28x28 grayscale images of handwritten digits. This project includes code for:
- Building and training the autoencoder.
- Visualizing the performance by plotting the loss curve.
- Visualizing original and reconstructed images.


## Autoencoder Overview

An autoencoder consists of two main parts:
- **Encoder:** The part of the network that compresses the input into a smaller representation.
- **Decoder:** The part that reconstructs the original input from the compressed data.

The encoder reduces the input dimensions into a latent space, while the decoder reconstructs the input from this space. The objective is to minimize the reconstruction loss, usually measured by Mean Squared Error (MSE).

### Model Architecture:
- **Input Layer:** 28x28 (784 units) for MNIST.
- **Encoder:** Fully connected layers reducing to a latent space of size 32.
- **Decoder:** Fully connected layers expanding back to 784 dimensions.
- **Output Layer:** Reconstructed 28x28 image.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/anantmehta33/Autoencoder.git
   cd Autoencoder

