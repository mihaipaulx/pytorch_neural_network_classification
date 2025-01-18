
# PyTorch Neural Network for Multiclass Classification

This repository demonstrates how to build, train, and evaluate a PyTorch-based neural network for multiclass classification. The project covers key aspects like data generation, model architecture, training loops, and performance visualization.

## Features

- **Custom Neural Network**: A three-layer feedforward model with ReLU activation for enhanced representation learning.
- **Dynamic Learning Rate Scheduling**: Implements a step learning rate scheduler for better optimization.
- **Visualization**: Provides decision boundary plots for training and testing data.
- **Evaluation**: Measures accuracy using PyTorch and TorchMetrics, achieving detailed performance tracking.

## Files

- `pytorch_neural_network_classification.py`: Main Python script containing all functionalities from data preprocessing to visualization.

## Requirements

The following Python libraries are required to run the code:

- `numpy`
- `pandas`
- `matplotlib`
- `torch`
- `torchmetrics`
- `scikit-learn`
- `jupyter`

Install the requirements with:
```bash
pip install numpy pandas matplotlib torchmetrics scikit-learn jupyter
```
For torch installation, check [Pytorch's official page](https://pytorch.org/get-started/locally/) 

## Project Workflow

1. **Data Generation**:
   - Creates synthetic multiclass datasets using `make_blobs` and `make_circles`.
   - Splits the data into training and testing sets.
   
2. **Model Architecture**:
   - Defines a customizable neural network with two hidden layers and ReLU activation.
   - Uses `CrossEntropyLoss` for multiclass classification tasks.

3. **Training and Evaluation**:
   - Includes a training loop with backpropagation and optimizer updates.
   - Evaluates performance using accuracy metrics for both training and testing datasets.

4. **Visualization**:
   - Plots decision boundaries to illustrate model predictions.

## Key Hyperparameters

- **Learning Rate**: Initial rate set at `0.01` (adjustable in the optimizer).
- **Epochs**: 50,000 iterations for training to ensure convergence.
- **Scheduler**: Reduces learning rate by 50% every 250 steps.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/mihaipaulx/pytorch_neural_network_classification.git
   cd your-repository
   ```
2. Run the script:
   ```bash
   jupyter notebook pytorch_neural_network_classification.ipynb
   ```
3. View the outputs, including:
   - Loss and accuracy metrics.
   - Decision boundary plots for train and test datasets.

## Example Results

| Epoch | Train Loss | Train Accuracy | Test Loss | Test Accuracy |
|-------|------------|----------------|-----------|---------------|
| 0     | 2.85005    | 0.75%          | 2.68741   | 1.00%         |
| 5000  | 0.13510    | 96.25%         | 0.16877   | 93.00%        |
| 45000 | 0.03195    | 98.75%         | 0.11071   | 96.00%        |

## Author

Mihai Paul Grinzeanu
