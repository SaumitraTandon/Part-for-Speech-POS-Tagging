# POS Tagging using Machine Learning

This project implements a Part-of-Speech (POS) tagging system using a machine learning model. The notebook preprocesses data, trains a neural network model for POS tagging, evaluates its performance, and compares it with a simple baseline model.

## Features

- **Data Preprocessing**: 
  - Tokenizes sentences into words.
  - Encodes words and POS tags as integers.
  - Pads sequences for uniform input size.
- **Neural Network Model**:
  - Implements an LSTM-based architecture for sequence modeling.
  - Trains the model on encoded data.
  - Visualizes training and validation performance metrics.
- **Evaluation**:
  - Computes accuracy and F1 score for train and test sets.
  - Evaluates the model with and without padding considerations.
- **Baseline Comparison**:
  - Implements a baseline model that maps each word to its most frequent tag.
  - Computes metrics to compare against the trained neural network.

## Getting Started

### Prerequisites

Make sure you have the following libraries installed:

- Python 3.7+
- NumPy
- TensorFlow/Keras
- scikit-learn
- Matplotlib
- NLTK
- Pandas

You can install these using `pip`:

```bash
pip install numpy tensorflow scikit-learn matplotlib nltk pandas
```

### Installation

1. Clone this repository:
    ```bash
    git clone <repository-url>
    cd <repository-folder>
    ```
2. Ensure all required libraries are installed.

### Dataset

The notebook assumes a dataset with sentences and their respective POS tags. Customize the data loading and preprocessing steps to fit your dataset format.

## Usage

1. Open the notebook `POS_Tagging.ipynb` in Jupyter or any compatible environment.
2. Execute the cells step by step to:
   - Load and preprocess the data.
   - Train the LSTM-based model.
   - Evaluate its performance.
   - Compare it with the baseline model.

### Key Functions

- `encode_sentences_and_tags`: Encodes sentences and their POS tags into integers.
- `pad_sequences`: Pads sequences to make them of uniform length.
- `create_model`: Defines the LSTM-based neural network architecture.
- `train_model`: Trains the neural network on the preprocessed dataset.

## Results

- **Model Accuracy**:
  - Train Accuracy: ~99.4%
  - Test Accuracy: ~97.3%
- **Model F1 Score**:
  - Train F1: ~0.99
  - Test F1: ~0.93
- **Baseline Metrics**:
  - Train Accuracy: ~95.7%
  - Test Accuracy: ~92.7%
  - Train F1: ~0.94
  - Test F1: ~0.83

The LSTM-based model significantly outperforms the baseline model in both accuracy and F1 score.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the code or documentation.

### Steps to Contribute

1. Fork this repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m "Added feature"`).
4. Push to your branch (`git push origin feature-branch`).
5. Open a pull request.

Feel free to reach out if you have questions or suggestions for improvement.
