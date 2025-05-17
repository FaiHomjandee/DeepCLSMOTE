# DeepCLSMOTE: Deep Class-Latent Synthetic Minority Oversampling Technique

  This repository contains the code for the DeepCLSMOTE method, a deep learning approach for handling imbalanced image datasets, as described in the paper "DeepCLSMOTE: Deep Class-Latent Synthetic Minority Oversampling Technique"
  DeepCLSMOTE is a deep learning-based image augmentation technique designed to address class imbalance in multi-class image classification. It extends the DeepSMOTE approach by explicitly optimizing the latent space using class centroids, leading to improved class separability and classification performance.


## 📦 Features

- Autoencoder-based latent feature generation
- Centroid-aware latent space optimization
- Integration with CNN classifiers
- Support for grayscale and RGB datasets
- Evaluated on six benchmark datasets with long-tailed distributions

## 🔧 Installation

```bash
git clone https://github.com/FaiHomjandee/DeepCLSMOTE.git
cd DeepCLSMOTE
pip install -r requirements.txt
