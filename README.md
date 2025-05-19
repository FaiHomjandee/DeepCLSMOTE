# DeepCLSMOTE: Deep Class-Latent Synthetic Minority Oversampling Technique

  This repository contains the code for the DeepCLSMOTE method, a deep learning-based image augmentation technique designed to address class imbalance in multi-class image classification. It extends the DeepSMOTE approach by explicitly optimizing the latent space using class centroids, leading to improved class separability and classification performance.

## Requirements:
PyTorch   
NumPy  
scikit-learn  

## Usage:
- Data preparation (transforms to tensor& gets imbalanced distribution).  
- Training Simple CNN with imbalanded dataset without autmentation then testing.  
- Training the DeepCLSMOTE model with imbalanced.   
- Generating synthetic samples based DeepSMOTE trained.  
- Training Simple CNN with balanded dataset then testing.  
- Evaluating the model is repeated via train-test datasets.  

## 🔧 Installation

```bash
git clone https://github.com/FaiHomjandee/DeepCLSMOTE.git
cd DeepCLSMOTE
pip install -r requirements.txt
```
## Usage

All the steps for data preparation, model training (both the baseline CNN and DeepCLSMOTE), synthetic sample generation (if applicable as a separate step), and evaluation are contained within the `DeepCLSMOTE.ipynb` Jupyter Notebook.

To run the experiments:

1.  **Open the Notebook:** Navigate to the repository directory in your terminal and open the `DeepCLSMOTE.ipynb` file using Jupyter Notebook or JupyterLab:

    ```bash
    jupyter notebook DeepCLSMOTE.ipynb
    # or
    jupyter lab DeepCLSMOTE.ipynb
    ```

2.  **Execute Cells:** Follow the instructions and execute the cells sequentially within the notebook. The notebook is structured to perform the following steps:
    * **Data Preparation:** Loads and preprocesses the image datasets, potentially creating imbalanced distributions as needed.
    * **Baseline CNN Training and Testing:** Trains a simple CNN on the imbalanced data and evaluates its performance.
    * **DeepCLSMOTE Training:** Trains the DeepCLSMOTE model on the imbalanced data.
    * **Synthetic Sample Generation (if applicable):** Generates synthetic minority class samples using a trained model (either DeepSMOTE as mentioned in your initial description or DeepCLSMOTE itself, depending on your implementation).
    * **Training CNN with Balanced Data:** Trains a CNN on the augmented (balanced) dataset.
    * **Evaluation:** Evaluates the performance of the models using appropriate metrics on train-test splits or through cross-validation as described in your paper.

3.  **Configuration:** You may need to modify certain variables within the notebook cells (e.g., file paths, hyperparameters, dataset parameters) to match your specific setup. Please refer to the comments within the notebook for guidance.

## File Structure  
DeepCLSMOTE/  
├── DeepCLSMOTE.ipynb     # Jupyter Notebook containing all the code  
├── README.md            # This file  
├── requirements.txt     # List of required packages  
├── data/                  # (Optional) Directory for datasets (adjust paths in notebook)  
└── models/                 # (Optional) Directory where trained models might be saved  
└── generated_images/       # (Optional) Directory for generated images  
