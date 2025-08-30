📝 Handwritten Digit Classification (MNIST Dataset)

This project focuses on classifying handwritten digits using the MNIST dataset. The dataset consists of 28×28 grayscale images of digits (0–9), and the goal is to build and train a neural network that can correctly recognize and classify these digits.

📌 Dataset Overview

Dataset: MNIST (Modified National Institute of Standards and Technology)

Images: 70,000 total (60,000 training, 10,000 testing)

Image Size: 28×28 pixels

Channels: 1 (grayscale)

Labels: Digits from 0 through 9

Each image is represented as pixel values (0–255), which are normalized to the range [0,1] for better training performance.

⚙️ Data Preprocessing

Loading Data:

(X_train, y_train), (X_test, y_test) = keras.datasets.mnist.load_data()


Training samples: 60,000

Testing samples: 10,000

Normalization:
Pixel values are scaled between 0 and 1:

X_train = X_train / 255
X_test = X_test / 255


Flattening:
Images (28×28) are reshaped into 1D vectors of length 784 to be fed into the input layer:

X_train_flattened = X_train.reshape(len(X_train), 28*28)
X_test_flattened = X_test.reshape(len(X_test), 28*28)

🏗️ Model Architecture

The model is a simple Feed-Forward Neural Network (FFNN) with one hidden layer:

Input Layer  →  Hidden Layer (ReLU)  →  Output Layer (Softmax)
   784               100                        10


Input Layer: 784 nodes (flattened 28×28 image)

Hidden Layer: 100 nodes with ReLU activation for non-linearity

Output Layer: 10 nodes with Softmax activation for digit classification

🚀 Training

Epochs: 5

Loss Function: Categorical Cross-Entropy

Optimizer: (Specify here: Adam/SGD, etc.)

Batch Size: (If applicable, specify)

📊 Results & Evaluation

✅ Test Accuracy: ~91%

📉 Confusion Matrix: Used to evaluate performance across classes

📈 Metrics Calculated:

Accuracy

Precision

Recall

F1 Score

🖼 Sample Prediction

Example output on a sample image:

True Label: 5
Predicted: 5


Visualization:

plt.matshow(X_train[0])
plt.show()