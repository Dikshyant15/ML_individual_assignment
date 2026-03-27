# ML_individual_assignment
Contains the file that is needed for the assignment, as the notebook file, and a report file.
Github Link: https://github.com/Dikshyant15/ML_individual_assignment/tree/main


=========================================================================================================================================================================

1. Project Overview

This project implements a convolutional denoising autoencoder combined with a CNN classifier for detecting breast cancer from histopathology images. The autoencoder learns robust, noise-resistant feature representations, which are then used to improve classification performance.

The approach focuses on:

Noise reduction in medical images
Learning meaningful latent features
Improving cancer vs non-cancer classification


=========================================================================================================================================================================

2. Methodology

The pipeline consists of:

Denoising Autoencoder
Learns to reconstruct clean images from noisy inputs
Extracts latent features (7×7×128)
Classifier
Uses encoded features as input
Applies CNN layers + Global Average Pooling
Predicts cancer probability using sigmoid output
Fine-Tuning
Unfreezes encoder
Improves feature learning for classification

=========================================================================================================================================================================

3. Results
Strong performance in cancer detection
Improved results after fine-tuning
Effective separation of classes in latent space (t-SNE visualization)


=========================================================================================================================================================================

4.  How to Run
i. Clone the repository
git clone git@github.com:Dikshyant15/ML_individual_assignment.git
cd ML_individual_assignment 
ii. Open Google Collab and upload the .ipynb file.
iii. Run the notebook
iv. Run all cells to reproduce results.
=========================================================================================================================================================================

5. Requirements

Python 3.x
TensorFlow / Keras
NumPy
Matplotlib
Scikit-learn

=========================================================================================================================================================================

6. Ethical Considerations
Model should be used as a decision-support tool only
Not a replacement for medical professionals
Risk of misclassification exists (especially false negatives)
Dataset bias may affect generalisation
=========================================================================================================================================================================

7. License
This project is licensed under the MIT License.