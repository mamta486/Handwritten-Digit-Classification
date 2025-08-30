📝 Handwritten Digit Classification

This project implements a Handwritten Digit Classification system using a simple feed-forward neural network trained on the MNIST dataset. The model is designed to recognize handwritten digits (0–9) with high accuracy.

📌 Project Overview

Input Layer: 784 nodes (for 28×28 grayscale images, flattened)

Hidden Layer: 100 nodes with ReLU activation to introduce non-linearity

Output Layer: 10 nodes (one for each digit class) with Softmax activation for classification

Training: Model trained for 10 epochs

Evaluation Metrics: Accuracy, Precision, Recall, and F1-score using a Confusion Matrix

⚙️ Model Architecture
Input Layer  →  Hidden Layer (ReLU)  →  Output Layer (Softmax)
   784               100                        10


Input Layer: Flattens 28×28 images into 784 features

Hidden Layer: Fully connected layer with 100 neurons, ReLU activation

Output Layer: Fully connected layer with 10 neurons, Softmax activation for multi-class classification

🚀 Training & Performance

Epochs: 10

Optimizer: (SGD/Adam – mention which you used)

Loss Function: Cross-Entropy Loss

Accuracy Achieved: ✅ ~97%

📊 Evaluation

A Confusion Matrix was used to calculate the following metrics:

✅ Accuracy

🎯 Precision

🔄 Recall

📈 F1 Score