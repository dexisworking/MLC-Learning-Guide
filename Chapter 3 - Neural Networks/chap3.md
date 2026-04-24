# 🤖 Chapter 3: Neural Networks (Brain Copycats)

> “Neural Networks are machines inspired by how we think.”

---

# 📌 1. What is a Neural Network?

A Neural Network is a computational model inspired by the **human brain**, made up of interconnected units called **neurons**.

\[
\text{Inputs} \rightarrow \text{Neurons} \rightarrow \text{Output}
\]

Each neuron processes information and passes it forward.

---

# 🧠 2. Biological vs Artificial Neuron

| Feature    | Biological Neuron | Artificial Neuron   |
| ---------- | ----------------- | ------------------- |
| Input      | Dendrites         | Input features      |
| Processing | Cell body         | Weighted sum + bias |
| Output     | Axon              | Activation output   |
| Signal     | Electrical        | Numerical           |

---

# ⚙️ 3. Artificial Neuron Model

## 📌 Components:

- Inputs: \(x_1, x_2, ..., x_n\)
- Weights: \(w_1, w_2, ..., w_n\)
- Bias: \(b\)
- Activation Function: \(f\)

---

## 🧮 Formula:

\[
z = \sum\_{i=1}^{n} w_i x_i + b
\]

\[
y = f(z)
\]

---

# 🔥 4. Activation Functions

Activation functions decide **whether a neuron should fire or not**.

---

## 📊 Common Functions

### 🔹 Sigmoid

\[
\sigma(x) = \frac{1}{1 + e^{-x}}
\]

- Output: (0, 1)
- Used in binary classification

---

### 🔹 ReLU (Rectified Linear Unit)

\[
f(x) = \max(0, x)
\]

- Fast and widely used
- Handles non-linearity

---

### 🔹 Tanh

\[
\tanh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}
\]

- Output: (-1, 1)

---

# 🏗 5. Neural Network Architecture

## 📌 Layers

| Layer           | Function        |
| --------------- | --------------- |
| Input Layer     | Receives data   |
| Hidden Layer(s) | Processes data  |
| Output Layer    | Produces result |

---

## 🔁 Data Flow

\[
\text{Input} \rightarrow \text{Hidden Layers} \rightarrow \text{Output}
\]

---

# 🧠 6. Deep Learning

When a network has **multiple hidden layers**, it is called:

\[
\text{Deep Neural Network}
\]

---

## 📌 Why Deep?

- Learns complex patterns
- Handles images, speech, NLP

---

# 🔄 7. Forward Propagation

## 📌 Definition:

Process of passing inputs through the network to get output.

---

## 🔁 Steps:

1. Input data enters network
2. Multiply with weights
3. Add bias
4. Apply activation
5. Pass to next layer

---

# 🔙 8. Backpropagation

## 📌 Definition:

Algorithm to update weights using error.

---

## 🧮 Error Function (Loss)

\[
L = (y - \hat{y})^2
\]

---

## 🔁 Steps:

1. Compute error
2. Propagate error backward
3. Update weights using gradient

---

# 📉 9. Gradient Descent

## 📌 Goal:

Minimize loss function

---

## 🧮 Update Rule:

\[
w = w - \alpha \frac{dL}{dw}
\]

Where:

- \( \alpha \) = learning rate

---

# ⚙️ 10. Important Concepts

## 🔹 Weights

- Represent importance of input
- Updated during training

---

## 🔹 Bias

- Helps shift the output

---

## 🔹 Epoch

- One full pass through dataset

---

## 🔹 Learning Rate

- Controls speed of learning

---

# 🧪 11. Special Neural Networks

## 🔹 Perceptron

- Single-layer neural network
- Used for simple classification

---

## 🔹 Autoencoder

### 📌 Purpose:

Compress and reconstruct data

\[
\text{Input} \rightarrow \text{Encoder} \rightarrow \text{Latent Space} \rightarrow \text{Decoder} \rightarrow \text{Output}
\]

---

# ⚖️ 12. Advantages & Limitations

## ✅ Advantages

- Handles complex patterns
- High accuracy
- Works on large data

---

## ❌ Limitations

- Requires large data
- Computationally expensive
- Hard to interpret

---

# 🧪 13. Real-World Applications

| Domain             | Use Case          |
| ------------------ | ----------------- |
| Computer Vision    | Face recognition  |
| NLP                | Chatbots          |
| Healthcare         | Disease detection |
| Autonomous Systems | Self-driving cars |

---

# 🧠 14. Intuition Summary

- Mimics human brain
- Learns patterns using layers
- Improves via error correction

---

# 🔥 15. Quick Recap

- Neural Network = interconnected neurons
- Key components:
  - Weights
  - Bias
  - Activation
- Processes:
  - Forward Propagation
  - Backpropagation
- Deep Learning = multiple layers

---

# 💡 16. Practice Ideas

- Build a perceptron
- Implement digit classifier (MNIST)
- Create simple autoencoder

---

# 🚀 Final Thought

Neural Networks are the backbone of modern AI.  
Master this, and you unlock Deep Learning.

---
