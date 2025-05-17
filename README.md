# DeepCLSMOTE: Deep Class-Latent Synthetic Minority Oversampling Technique

  This repository contains the code for the DeepCLSMOTE method, a deep learning-based image augmentation technique designed to address class imbalance in multi-class image classification. It extends the DeepSMOTE approach by explicitly optimizing the latent space using class centroids, leading to improved class separability and classification performance.

## 📦 Features
- Autoencoder-based latent feature generation
- Centroid-aware latent space optimization
- Integration with CNN classifiers
- Support for grayscale and RGB datasets
- Evaluated on six benchmark datasets with long-tailed distributions

## Requirements:
PyTorch 
NumPy
scikit-learn

## Usage:
Data preparation (transforms to tensor& gets imbalanced distribution).
Training Simple CNN with imbalanded dataset without autmentation then testing.
Training the DeepCLSMOTE model with imbalanced. 
Generating synthetic samples based DeepSMOTE trained.
Training Simple CNN with balanded dataset then testing.
Evaluating the model is repeated via train-test datasets.

## 🔧 Installation

```bash
git clone https://github.com/FaiHomjandee/DeepCLSMOTE.git
cd DeepCLSMOTE
pip install -r requirements.txt
