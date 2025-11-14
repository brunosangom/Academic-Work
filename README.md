# Academic Work

This repository contains a collection of academic works completed during my Bachelor's and Master's degrees, focusing on advanced topics in machine learning, neural networks, and intelligent systems.

## Master's Thesis (WIP)

**Concept Drift-aware Federated Continual Learning for Spacecraft Prognostics and Health Management**

This paper proposes a novel framework that integrates Federated Learning (FL), Continual Learning (CL), and Concept Drift (CD) detection for Anomaly Detection in satellite telemetry.

* **Core Problem:** Addresses key PHM challenges in spacecraft constellations, including data privacy (using FL), model adaptation to evolving data streams (using CL), and inefficient periodic retraining (using CD-triggered updates).
* **Methodology:** Employs an LSTM-based model (Telemanom) for time-series forecasting. Anomalies are subsequently identified by applying a threshold to the model's prediction errors.
* **Update Strategy:** Compares a standard "Synchronous Periodic Retraining" FCL strategy against an "Asynchronous Drift-Triggered Retraining" approach. The asynchronous method uses client-side ADWIN and Page-Hinkley (PH) tests to detect concept drift and initiate model updates.
* **Evaluation:** The framework is validated on a confidential "Constellation Dataset" from a real-world fleet of satellites, with hyperparameters tuned using the public ESA-ADB dataset.
* **Analysis:** Investigates the performance trade-off between using the aggregated global model for inference versus using a locally fine-tuned "personalized" model on each client.

## Bachelor's Thesis

**Mathematical Modeling and Practical Application of Transformer Neural Networks**

This thesis constructs a unified mathematical framework for neural networks based on function spaces and provides a deep dive into the mathematical modeling of the Transformer architecture.

* **Core Concept:** Proposes a formal framework that defines a neural network as a parameterized function and the training process as a variational problem on the network's function space. This is then reduced to a solvable optimization problem on the parameter space.
* **Architectural Breakdown:** Provides a detailed mathematical definition of each component of the Transformer architecture, including the Embedding layer, Multi-Head Attention (self- and cross-attention), Addition & Normalization layers, and the final Perceptron layer.
* **Training and Optimization:** Details the use of the cross-entropy error function (via log-softmax) for sequence transduction tasks. It also derives the complete back-propagation algorithm, calculating the specific gradients for every parameter in the Transformer's layers.
* **Practical Application:** Implements the framework in C++ to build and train a Transformer model for an English-to-Spanish translation task.
* **Results:** Compares the training performance (e.g., time, epochs to converge) and testing accuracy of three different model configurations ("Small," "Medium," and "Large") to analyze the impact of architecture size.
