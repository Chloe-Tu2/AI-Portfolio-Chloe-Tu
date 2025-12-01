# CNN: Chihuahua vs. Muffin Classification

## Project Overview
**Module:** 07 - Convolutional Neural Networks (CNN)  

**Task:** Binary Image Classification  

**Framework:** PyTorch  

This project tackles a classic and humorous computer vision challenge: distinguishing between **Chihuahuas** and **Blueberry Muffins**. While trivial for humans, this task is notoriously difficult for AI due to high **inter-class similarity** (round shapes, similar tan/brown textures, and button-like features representing eyes or blueberries). I designed and trained a custom **Convolutional Neural Network (CNN)** to solve this problem, analyzing performance over 10 epochs and modifying the training function to optimize convergence.

## Problem Statement
* **Visual Similarity:** The model must distinguish subtle anatomical features (ears, snouts) from food textures, despite both classes having nearly identical color histograms.
* **Optimization Challenge:** Balancing the learning rate and batch size to ensure the model generalizes rather than memorizing the small dataset.
* **Goal:** To achieve stable validation accuracy and minimize loss across extended training epochs.

## Approach & Methodology

### 1. Data Pipeline
* **Preprocessing:** Resized images and converted them to PyTorch tensors.
* **Split:** Divided data into Training (80%) and Validation (20%) sets.
* **DataLoader:** Implemented a custom loader to handle batching, shuffling, and image transformations.

### 2. CNN Architecture
* **Convolutional Layers:** Extracted spatial features (edges -> textures -> object parts).
* **Pooling:** Reduced spatial dimensions to focus on dominant features.
* **Fully Connected Layers:** Performed final binary classification.

### 3. Training Experiments
* **Standard Training:** Ran an initial baseline training loop for 5 epochs.
* **Extended Training:** Continued training from Epoch 6-10 to observe long-term convergence.
* **Modified Training Function:** Experimented with adjustments to the training loop (e.g., logging frequency, loss tracking) to better visualize the "Learning Curve."

## Results & Visualizations

### 1. Setup & Architecture
Visualizing the foundational components of the PyTorch pipeline.

| Training Setup | Data Preparation | Model Definition |
|:---:|:---:|:---:|
| ![Setup](Results-&-Visualizations/Training_Setup.png) | ![Split](Results-&-Visualizations/Data_Preparation_Train-Test%20Split.png) | ![Model](Results-&-Visualizations/Model_Definition.png) |
| *Hyperparameters & Device* | *Train/Test Data Split* | *Layer Architecture* |

### 2. Training Progression (Epochs 1-10)
Tracking the model's accuracy and loss reduction over time.

| Epochs 1-5 (Initial) | Epochs 6-10 (Extended) |
|:---:|:---:|
| ![Epoch 1-5](Results-&-Visualizations/Model_Trainning_Epoch_1-5.png) | ![Epoch 6-10](Results-&-Visualizations/Model_Trainning_Epoch_6-10.png) |

### 3. Modified Training Function Analysis
Results from the optimized training loop experiments.

| Modified Epochs 1-5 | Modified Epochs 6-10 |
|:---:|:---:|
| ![Mod Epoch 1-5](Results-&-Visualizations/Modify_The_Training_Function_Epoch_1-5.png) | ![Mod Epoch 6-10](Results-&-Visualizations/Modify_The_Training_Function_Epoch_6-10.png) |

### 4. Loss Analysis & Evaluation
Visualizing the "Generalization Gap" between training and validation performance.

| Loss Visualization 1 | Loss Visualization 2 |
|:---:|:---:|
| ![Loss 1](Results-&-Visualizations/Visualize_Training_Progress_Training_and_Validation_Loss_per_Epoch_1.png) | ![Loss 2](Results-&-Visualizations/Visualize_Training_Progress_Training_and_Validation_Loss_per_Epoch_2.png) |

| Comparative Analysis | Final Prediction |
|:---:|:---:|
| ![Compare](Results-&-Visualizations/Analyze_Compare_Results_Training_and_Validation_Loss_Comparison_1.png) | ![Eval](Results-&-Visualizations/Model_Evaluation_Chihuahua_and_Muffin.jpg) |

## Key Findings
1.  **Convergence:** The model showed rapid learning in the first 3 epochs but required careful tuning (seen in Epochs 6-10) to prevent the validation loss from plateauing or increasing (overfitting).
2.  **Modified Function:** Adjusting the training function provided clearer granular logs, helping to identify exactly when the model started to memorize the data vs. learning features.
3.  **Visual Distinction:** Despite the difficulty, the CNN successfully identified "Muffin" vs "Chihuahua" in the test set (as seen in the Evaluation image), proving that convolution filters can separate texture (muffin top) from anatomy (dog eyes).

## Technologies Used
* **Python 3.8+**
* **PyTorch:** `torch`, `torch.nn`, `torch.optim` for deep learning.
* **Matplotlib:** For visualizing loss curves and sample predictions.
* **Pandas/NumPy:** For data structure handling.
* **Scikit-Learn:** For dataset splitting.

## Project Structure

```text
Project-07-CNN-Chihuahua-or-Muffin/
├── P07_CNN-Chihuahua-or-Muffin.ipynb       # Main PyTorch Notebook
├── P07_PF_CNN-Chihuahua-or-Muffin.pdf      # Project Report
├── J07_RF_CNN-Chihuahua-or-Muffin.pdf      # Reflection Journal
├── README.md                               # Project Documentation
└── Results-&-Visualizations/               # All Output Images
    ├── Analyze_Compare_Results_Training_and_Validation_Loss_Comparison_1.png
    ├── Analyze_Compare_Results_Training_and_Validation_Loss_Comparison_2.png
    ├── Data_Preparation_Train-Test Split.png
    ├── Dataset_and_Dataloader.png
    ├── Model_Definition.png
    ├── Model_Evaluation_Chihuahua_and_Muffin.jpg
    ├── Model_Trainning_Epoch_1-5.png
    ├── Model_Trainning_Epoch_6-10.png
    ├── Modify_The_Training_Function_Epoch_1-5.png
    ├── Modify_The_Training_Function_Epoch_6-10.png
    ├── Training_Setup.png
    ├── Visualize_Training_Progress_Training_and_Validation_Loss_per_Epoch_1.png
    └── Visualize_Training_Progress_Training_and_Validation_Loss_per_Epoch_2.png
