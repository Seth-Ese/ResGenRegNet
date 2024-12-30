

# ResGenRegNet: A Residual Block-Based Approach for Early Detection of Lung Cancer

## Overview
ResGenRegNet is a deep learning-based framework designed to enhance the early detection of lung cancer. By leveraging residual blocks and regularisation techniques, this model addresses the challenges of traditional methods, such as vanishing gradients and imbalanced datasets, to achieve state-of-the-art accuracy in distinguishing between benign and malignant stages of lung cancer.

## Features
- **Residual Block Architecture**: Efficiently handles vanishing gradient issues in deep networks.
- **Advanced Regularisation**: Incorporates L2 regularisation and dropout in each layer to enhance generalisation and mitigate overfitting.
- **Dataset Versatility**: Validated on multiple datasets, including IQ-OTH/NCCD and Pneumonia Chest X-ray Images, demonstrating robust performance across diverse data.
- **High Performance**:
  - Achieved 98% accuracy on the IQ-OTH/NCCD dataset with 5-fold cross-validation.
  - Achieved 96.55% accuracy on the Pneumonia Chest X-ray dataset.

## Objectives
1. Enhance the accuracy of lung cancer detection using advanced deep learning techniques.
2. Address common challenges like imbalanced datasets through oversampling (SMOTE) and data augmentation.
3. Develop a versatile model applicable to various medical imaging datasets.

## Technologies Used
- **Programming Language**: Python
- **Deep Learning Frameworks**: TensorFlow, Keras
- **Data Preprocessing**: ImageDataGenerator, SMOTE
- **Architecture**: Residual Networks (ResNet)
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, ROC-AUC

## Datasets
1. **IQ-OTH/NCCD Dataset**: CT scan images for lung cancer detection.
2. **Pneumonia Chest X-ray Images**: Used for cross-validation and diversity testing.

## Methodology
1. **Data Preprocessing**:
   - Rescaled and standardised images for consistency.
   - Applied SMOTE to balance dataset classes.
2. **Model Architecture**:
   - Built on the ResNet framework.
   - Utilised 3x3 convolutional filters, batch normalisation, and activation functions.
   - Introduced L2 regularisation and dropout in all layers for robust learning.
   - Incorporated skip connections to ensure gradient flow and improve learning efficiency.
3. **Evaluation**:
   - Performed ablation studies to assess the impact of architectural components.
   - Validated the model through 5-fold cross-validation and metrics like sensitivity, specificity, and AUC.

## Results
- **IQ-OTH/NCCD Dataset**:
  - Accuracy: 98%
  - Sensitivity: 96.49%
  - Specificity: 100%
- **Pneumonia Chest X-ray Dataset**:
  - Accuracy: 96.55%
  - High classification precision, recall, and F1-scores across all classes.

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/Seth-Ese/ResGenRegNet.git
   cd ResGenRegNet
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the project:
   ```bash
   python train_model.py
   ```

## Usage
- Update dataset paths in the configuration file.
- Run the training script to train the model on your dataset.
- Evaluate the model using the provided evaluation script.

## Future Work
- Extend the model to detect other types of cancer.
- Integrate the framework into a user-friendly application for medical professionals.

## Repository Link
Find the full implementation [here](https://github.com/Seth-Ese/ResGenRegNet).

---

Let me know if you'd like adjustments or additional sections!

### Training and validation Curve
![image](https://github.com/user-attachments/assets/ce59657c-18a3-4edc-ada8-52cc6c3f4fe6)

### Acknowledgments
This work has been accomplished with the support and guidance of Dr. Sandeep Singh Sengar at Cardiff School of Technologies, Cardiff Metropolitan University.
