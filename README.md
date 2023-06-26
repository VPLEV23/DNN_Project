# DNN PRoject

## Overview
The project aims to compare the performances of two sets of three Convolutional Neural Networks (CNNs) by coding and in the report. The CNNs in each set share the same architecture but differ in their training/initialization schema. The performance comparisons are based on the MNIST 2-D dataset, and the CNNs are built and trained using the PyTorch library.

## Technical Requirements
- Library: PyTorch
- Dataset: MNIST 2-D dataset
- Code: Python file or Jupyter Notebook
- Report: PDF file describing the experiments, including results, analysis, and personal comments

## CNN Architectures
### Set 1: A1
- CNN Architecture:
  - One convolutional layer with 4 kernels
  - One fully connected layer
  - One Softmax output layer
  - Cross entropy loss

### Set 2: A2
- CNN Architecture:
  - One convolutional layer with 4 kernels
  - One additional convolutional layer (number of kernels of your choice)
  - Optionally, more convolutional layers can be added
  - One fully connected layer
  - One Softmax output layer
  - Cross entropy loss

Note: Kernel sizes and activation functions for the hidden layers should be decided.

## Training/Initialization Schemas
  - HF Schema:
    - The first layer is initialized with the by-hand strategy
    - The remaining layers are initialized with the default strategy
    - All layers except the first one (Frozen layer) are trained
  - HT Schema:
    - The first layer is initialized with the by-hand strategy
    - The remaining layers are initialized with the default strategy
    - All layers, including the first one, are trained
  - DT Schema:
    - All layers, including the first one, are initialized with the default strategy
    - All layers, including the first one, are trained
## Experiments and Comparisons
1. In-Set Comparison:
   - Compare the performances (loss and accuracy at each epoch) of all the CNNs within each set (A1 or A2) to understand the impact of the training/initialization schema while keeping the architecture fixed.

2. Architecture Comparison:
   - Compare the performances (loss and accuracy at each epoch) of CNNs with different architectures while maintaining the same training/initialization schema.

3. Recovery Comparison:
   - Compare the performances (loss and accuracy at each epoch) of A2-HF to all the CNNs in Set 1 (A1-*). Compare the following pairs:
     - A2-HF/A1-HF
     - A2-HF/A1-HT
     - A2-HF/A1-DT

## How to Use
1. Clone the repository.
2. Install the required libraries.

   ```bash
    pip install -r requirements.txt
4. Run the Python file or Jupyter Notebook containing the code for the experiments.
5. Refer to the report (PDF file) for detailed analysis, results, and personal comments on the conducted experiments.

## Author
Your Name

## License
This project is licensed under the [License Name] - [License URL] (if applicable)
