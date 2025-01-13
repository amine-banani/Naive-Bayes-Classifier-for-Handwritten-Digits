# Naive Bayes Classifier for Handwritten Digits

This project implements a **Naive Bayes Classifier** for recognizing handwritten digits from the **MNIST dataset**, supporting both discrete and continuous feature modes. The dataset is manually parsed to better understand its format and avoid reliance on pre-built datasets.

---

## Features

1. **Naive Bayes Classification**:
   - **Discrete Mode**: 
     - Divides pixel values into 32 bins and computes frequencies for classification.
     - Includes pseudocounts to handle empty bins.
   - **Continuous Mode**:
     - Fits pixel values to Gaussian distributions using Maximum Likelihood Estimation (MLE).

2. **MNIST Dataset Parsing**:
   - Manual parsing of training and testing data (images and labels) in big-endian binary format.

3. **Outputs**:
   - Posterior probabilities (log scale) for each digit (0-9) per test image.
   - Predicted labels with error rate calculation.
   - Visual representation of the digits in the Bayes classifier:
     - Binary images where pixels are classified as black (1) or white (0) based on thresholds.
