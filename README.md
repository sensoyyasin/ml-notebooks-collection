# Machine Learning Notebooks — Assignment III
**California State University, Chico** | Machine Learning Course

---

## Overview

A collection of machine learning notebooks covering **Supervised Learning** (SVM, ANN, MLP) and **Reinforcement Learning** (CartPole). Implemented using Python, TensorFlow/Keras, and Scikit-learn.

---

## Projects

### 1. Support Vector Machines (SVM)
- Linear SVM Classification with feature scaling analysis
- Nonlinear SVM using RBF, Polynomial, and Sigmoid kernels
- Soft Margin vs Hard Margin comparison
- Hyperparameter tuning: C, Gamma, Kernel type
- Key finding: RBF kernel with `gamma=scale` and small C performs best on noisy nonlinear data

<img width="759" height="608" alt="Ekran Resmi 2026-02-28 11 38 48" src="https://github.com/user-attachments/assets/b3d56c2e-8ed6-4039-9814-6c37d4af2206" />


<img width="781" height="170" alt="Ekran Resmi 2026-02-28 11 39 15" src="https://github.com/user-attachments/assets/016b978d-6aae-400c-9e40-b4cf6893d8f6" />





### 2. Artificial Neural Networks (ANN)
- Built with Keras Sequential API
- Fashion MNIST dataset (10-class classification)
- Trained with SGD optimizer and Sparse Categorical Crossentropy loss
- Analysis of overfitting between 30 and 50 epochs
- Architecture: Flatten → Dense(1000, ReLU) → Dense(100, ReLU) → Dense(10, Softmax)

<img width="651" height="363" alt="Ekran Resmi 2026-02-28 11 39 35" src="https://github.com/user-attachments/assets/b0e9fde6-37c1-4644-a10f-8026e180c468" />

<img width="736" height="326" alt="Ekran Resmi 2026-02-28 11 40 11" src="https://github.com/user-attachments/assets/1d37af7c-1d28-4103-aca7-5e11d0cd63ac" />

<img width="601" height="281" alt="Ekran Resmi 2026-02-28 11 40 24" src="https://github.com/user-attachments/assets/0f894124-87b3-4523-beed-3d5c512307da" />


<img width="558" height="377" alt="Ekran Resmi 2026-02-28 11 40 33" src="https://github.com/user-attachments/assets/b5a02018-a68d-487a-b8c8-13933c4fa9d6" />

<img width="575" height="381" alt="Ekran Resmi 2026-02-28 11 40 45" src="https://github.com/user-attachments/assets/b9da7d63-56a4-4bf2-ad15-ce882a2315db" />



### 3. Multilayer Perceptron (MLP)
- Deep dive into backpropagation, vanishing gradients, and activation functions
- Comparison of ReLU vs Sigmoid vs Tanh
- Fashion MNIST classification
- Architecture: 784 → 300 → 100 → 10

### 4. Reinforcement Learning (CartPole)
- Rule-based policy vs ANN Policy Gradient
- Rule-based average reward: 159.5 / 200
- ANN achieved perfect mean reward of 200.0 at iteration 28/100
- Architecture: Dense(32, ReLU) → Dense(32, ReLU) → Dense(1, Sigmoid)

---

## Results Summary

| Model | Dataset | Accuracy / Reward |
|-------|---------|-------------------|
| SVM (RBF, C=0.1) | make_circles | 87.78% |
| ANN (50 epochs) | Fashion MNIST | Val Accuracy: 88.30% |
| MLP | Fashion MNIST | Val Accuracy: ~88% |
| Rule-based Policy | CartPole | 159.5 / 200 |
| ANN Policy Gradient | CartPole | 200.0 / 200|

---

## Tech Stack

- Python
- Scikit-learn
- TensorFlow / Keras
- NumPy, Matplotlib
- OpenAI Gymnasium (CartPole)

---

## Topics

`machine-learning` `svm` `ann` `mlp` `reinforcement-learning` `tensorflow` `scikit-learn` `python` `fashion-mnist` `cartpole` `keras`

---

## References

- Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow — Aurélien Géron
- [Scikit-learn Scaling Docs](https://scikit-learn.org/stable/auto_examples/preprocessing/plot_scaling_importance.html)
- [Gymnasium CartPole](https://gymnasium.farama.org/introduction/basic_usage/)
