# Quantum Machine Learning: A Simple Classifier

This project builds a Quantum Support Vector Machine (QSVM) to classify a simple 2D dataset. It demonstrates the full workflow of a QML project using Qiskit.

## 1. Objective
The goal is to show how a quantum circuit can be used as a "kernel" to help a classical machine learning algorithm (an SVC) classify data that is not easily separable.

The workflow is:
1.  **Load Data**: Import a simple, non-linearly separable dataset (`ad_hoc_data`).
2.  **Define Quantum Kernel**: Create a `ZZFeatureMap` to map the classical data into a quantum feature space.
3.  **Build Kernel**: Use the `FidelityQuantumKernel` to make this map usable by the classifier.
4.  **Train**: Train a classical `SVC` using this quantum kernel.
5.  **Evaluate**: Test the model's accuracy on unseen data.

## 2. Technologies Used
* Python
* Qiskit
* Qiskit Machine Learning
* Qiskit Algorithms
* Scikit-learn
* Matplotlib
* NumPy

## 3. How to Run
1.  Clone the repository.
2.  Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```
3.  Open and run the `QML Classifier.ipynb` file in a Jupyter environment.

## 4. Key Results
The notebook successfully trains the classifier and scores it on the test set.

*(Note: The low accuracy, e.g., ~40%, is expected. This project demonstrates the workflow, not state-of-the-art performance, which would require a much larger dataset and kernel optimization.)*
