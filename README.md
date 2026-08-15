# Neural Network Implementation from Scratch - XOR

## Student Information

- **Name:** Parth Kitchloo
- **PRN Number:** 202401110014
- **Batch:** A2
- **Course:** Generative AI Lab
- **Department:** CSE AIML
- **Date of Submission:** 15 August 2026

---

## 1. Objective

The objective of this project is to implement a simple feedforward neural network
from scratch using Python and NumPy.

The implementation demonstrates:

- Forward propagation
- Sigmoid activation
- Mean Squared Error (MSE)
- Backpropagation
- Gradient descent
- Model training
- Prediction and evaluation

No deep learning frameworks such as TensorFlow, Keras, or PyTorch are used.

---

## 2. Problem Definition

The XOR (Exclusive OR) logic gate is used as the dataset.

XOR produces an output of 1 when the two input values are different
and produces an output of 0 when the two input values are the same.

| Input 1 | Input 2 | Output |
|---------|---------|--------|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

XOR is a non-linearly separable problem, so a hidden layer is required
to learn the relationship.

---

## 3. Neural Network Architecture

The implemented neural network uses the following architecture:

**2 → 2 → 1**

- Input Layer: 2 neurons
- Hidden Layer: 2 neurons
- Output Layer: 1 neuron
- Activation Function: Sigmoid
- Loss Function: Mean Squared Error
- Optimization: Gradient Descent

---

## 4. Methodology

### Forward Propagation

The input data is passed through the hidden layer and then the output layer.

The calculations are:

Z1 = XW1 + b1

A1 = Sigmoid(Z1)

Z2 = A1W2 + b2

A2 = Sigmoid(Z2)

### Backpropagation

Backpropagation is used to calculate the gradients of the weights and
biases with respect to the loss.

The gradients are propagated from the output layer back towards the
hidden layer.

### Gradient Descent

The weights and biases are updated using:

W = W - Learning Rate × Gradient

This process is repeated for multiple epochs to minimize the loss.

---

## 5. Training Configuration

- **Epochs:** 10,000
- **Learning Rate:** 0.5
- **Activation Function:** Sigmoid
- **Loss Function:** Mean Squared Error
- **Network Architecture:** 2-2-1

---

## 6. Model Evaluation

After training, the model predicts the four XOR input combinations.

The predicted probability is converted into a binary prediction using
a threshold of 0.5.

- Prediction >= 0.5 → 1
- Prediction < 0.5 → 0

The model performance is evaluated using:

- Mean Squared Error
- Accuracy
- Actual vs Predicted values

---

## 7. Single-Layer Comparison

A single-layer neural network with a **2-1 architecture** is also implemented
for comparison.

The comparison demonstrates the importance of a hidden layer when solving
the non-linearly separable XOR problem.

The training loss of both models is also compared using a graph.

---

## 8. Visualization

The project includes:

- Training Loss vs Epochs graph
- Loss comparison between the single-layer and 2-2-1 neural networks
- Final prediction results

---

## 9. Technologies Used

- Python
- NumPy
- Matplotlib
- Google Colab
- GitHub

---

## 10. Files

- `Parth_Kitchloo_GenerativeAILabAssignment.ipynb` - Complete implementation
- `README.md` - Project documentation
- `requirements.txt` - Required Python libraries

---

## 11. Conclusion

This project demonstrates how a feedforward neural network can be implemented
from scratch without using a deep learning framework.

The experiment shows the importance of hidden layers and non-linear activation
functions for learning the XOR relationship.

The implementation covers the complete basic neural network training process:

**Forward Propagation → Loss Calculation → Backpropagation → Gradient Descent → Prediction**

---

## 12. Author

**Parth Kitchloo**

MIT Academy of Engineering, Pune  
CSE AIML
