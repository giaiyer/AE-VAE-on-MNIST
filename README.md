# AE and VAE on MNIST Dataset
 
This project implements and compares **Autoencoder (AE)** and **Variational Autoencoder (VAE)** models on the MNIST dataset using PyTorch. The focus is on image reconstruction, denoising capability, latent space visualization, and interpolation between digits.

## Features

- **Denoising Autoencoder (AE)**
- **Denoising Variational Autoencoder (VAE)**
- **Latent space visualization** using t-SNE / PCA
- **Random generation** from VAE latent space
- **Interpolation** between digit pairs in latent space
- **Clustering analysis** with K-Means and ARI score
- **Side-by-side AE vs VAE reconstruction comparison**

## Models

### Autoencoder (AE)
- Encoder: Fully connected layers compress input to latent vector
- Decoder: Reconstructs image from latent representation
- Loss: MSE
- Includes noise injection for **denoising**

### Variational Autoencoder (VAE)
- Encoder: Outputs `μ` and `log(σ²)` for each image
- Sampling: Reparameterization trick
- Decoder: Generates image from sampled latent vector
- Loss: Binary Cross-Entropy + KL Divergence
- Can **generate new digits** from random samples

---
