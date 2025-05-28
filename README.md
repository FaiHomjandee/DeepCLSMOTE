# DeepCLSMOTE: Deep Class-Latent Synthetic Minority Oversampling Technique

  This repository contains the code for the DeepCLSMOTE method, a deep learning-based image augmentation technique designed to address class imbalance in multi-class image classification. It extends the DeepSMOTE approach by explicitly optimizing the latent space using class centroids, leading to improved class separability and classification performance.
  
## Datasets
This implementation was evaluated on the following publicly available image datasets
[Provide URL or citation if you explicitly downloaded it from a specific source]:
* MNIST  [http://yann.lecun.com/exdb/mnist/](http://yann.lecun.com/exdb/mnist/)
* Fashion-MNIST
* EMNIST
* SVHN
* GTSRB
* CIFAR-10

## Code Information
The main files in this repository are:
DeepCLSMOTE/  
├── DeepCLSMOTE.ipynb     # Jupyter Notebook containing all the code  
├── README.md            # This file 

## Usage Instructions
All the steps for data preparation, model training (both the baseline CNN and DeepCLSMOTE), synthetic sample generation , and evaluation are contained within the `DeepCLSMOTE.ipynb` Jupyter Notebook.

To run the experiments:

1.  **Open the Notebook:** Navigate to the repository directory in your terminal and open the `DeepCLSMOTE.ipynb` file using Jupyter Notebook or JupyterLab:

    ```bash
    jupyter notebook DeepCLSMOTE.ipynb
    # or
    jupyter lab DeepCLSMOTE.ipynb
    ```

2.  **Execute Cells:** Follow the instructions and execute the cells sequentially within the notebook. The notebook is structured to perform the following steps:
    * **Data Preparation:** Loads the image datasets, potentially creating imbalanced distributions as needed.
    * **Baseline CNN Training and Testing:** Trains a simple CNN on the imbalanced data and evaluates its performance.
    * **DeepCLSMOTE Training:** Trains the DeepCLSMOTE model on the imbalanced data.
    * **Synthetic Sample Generation :** Generates synthetic minority class samples using a trained DeepCLSMOTE.
    * **Training CNN with Balanced Data:** Trains a CNN on the augmented (balanced) dataset.
    * **Evaluation:** Evaluates the performance of the models using appropriate metrics on train-test splits or through cross-validation as described in the paper.

3.  **Configuration:** You may need to modify certain variables within the notebook cells (e.g., file paths, dataset parameters) to match your specific setup.

## Requirements:
PyTorch   
NumPy  
scikit-learn  

## Citations: 
If you use this code in your research, please cite the following reference:
> Homjandee, S. and Sinapiromsaran, K. (2025). Deepclsmote: Deep class-latent synthetic minority oversampling technique. https://doi.org/10.5281/zenodo.15362173. Code repository archived on Zenodo.
 
