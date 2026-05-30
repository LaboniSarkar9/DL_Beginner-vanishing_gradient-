# DL_Beginner-vanishing_gradient-
Binary classification of the Moon Dataset using TensorFlow/Keras, highlighting the vanishing gradient problem associated with sigmoid activation functions in deep neural networks.

# Moon Dataset Classification using Neural Network

## Project Overview

This project demonstrates binary classification using a Neural Network built with TensorFlow/Keras. The model is trained on the Moon Dataset generated using Scikit-learn's `make_moons()` function.

## Dataset

The dataset consists of two interleaving moon-shaped classes and is commonly used to evaluate classification algorithms.

* Samples: 250
* Features: 2
* Classes: 2
* Noise: 0.05

## Steps Performed

### 1. Import Required Libraries

Imported NumPy, Pandas, Matplotlib, TensorFlow/Keras, and Scikit-learn libraries.

### 2. Generate Dataset

Created the Moon Dataset using:

```python
X, y = make_moons(n_samples=250, noise=0.05, random_state=42)
```

### 3. Train-Test Split

Split the dataset into training and testing sets for model evaluation.

### 4. Build Neural Network

Constructed a Sequential Neural Network with:

* Input Layer: 2 features
* Hidden Layer(s): Dense layers with ReLU/Sigmoid activation
* Output Layer: 1 neuron with Sigmoid activation

### 5. Compile Model

Configured the model using:

* Optimizer: Adam
* Loss Function: Binary Crossentropy
* Metric: Accuracy

### 6. Train Model

Trained the model for multiple epochs to learn decision boundaries.

### 7. Evaluate Performance

Measured model accuracy on the test dataset.

### 8. Visualize Results

Plotted the dataset and analyzed model performance using training metrics.

## Technologies Used

* Python
* TensorFlow / Keras
* Scikit-learn
* NumPy
* Pandas
* Matplotlib

## Results

The neural network successfully learns the non-linear decision boundary of the Moon Dataset and achieves good classification accuracy.

## How to Run

```bash
pip install tensorflow scikit-learn numpy pandas matplotlib
```

Run the Jupyter Notebook or Python script:

```bash
python moon_classification.py
```
