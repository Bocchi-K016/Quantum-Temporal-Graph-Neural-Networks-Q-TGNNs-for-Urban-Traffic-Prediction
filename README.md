# Quantum Temporal Graph Neural Networks (Q-TGNNs) for Urban Traffic Prediction

## Project Overview
An innovative approach to urban traffic prediction combining Quantum Computing with Temporal Graph Neural Networks (TGNN). This project implements two quantum-enhanced models to improve traffic forecasting accuracy while exploring the potential of quantum machine learning in real-world applications.

## Description:
This project presents Quantum Temporal Graph Neural Networks (Q-TGNNs), a novel approach combining the strengths of Quantum Computing and Graph Neural Networks (GNNs) for enhanced urban traffic prediction. Urban traffic congestion, with its significant environmental and economic costs, demands models that can handle the complex, time-varying nature of road networks. By integrating quantum computing with temporal GNNs, this project aims to achieve more precise traffic predictions, supporting real-time traffic management in smart cities.

## Project Background
Traditional traffic models are limited in capturing the dynamic and spatially-connected patterns of urban traffic flow. The Q-TGNN model leverages Quantum Computing principles—such as superposition and entanglement—alongside GNNs to address these challenges. The METR-LA dataset, containing traffic data from the Los Angeles metropolitan area, serves as the primary dataset, offering both spatial and temporal features essential for training and validating the Q-TGNN.

## Model Architecture
The project explores two major Q-TGNN architectures:
- Basic Quantum Layer-Enhanced Temporal GNN: This model combines classical GNN layers with a simple 2-qubit quantum layer, using PauliX and PauliZ operations to capture high-order temporal relationships.
- Enhanced Quantum Layer Temporal GNN: Building on the basic model, this version adds advanced quantum optimizations, such as the Quantum Approximate Optimization Algorithm (QAOA) and Gaussian kernel edge weights, to refine message passing and capture complex data patterns.
Each model includes classical components based on the A3TGCN2 architecture for spatial-temporal feature extraction, along with quantum layers for high-dimensional data processing.

## Key Features
- Integration of quantum computing with classical Graph Neural Networks
- Two quantum-enhanced architectures:
  - Basic Q-TGNN with 2-qubit quantum circuit using AngleEmbedding and StronglyEntanglingLayers
  - Enhanced Q-TGNN incorporating QAOA and Gaussian kernel edge weights
- Temporal traffic prediction using the METR-LA dataset
- Hybrid classical-quantum architecture leveraging PyTorch, PennyLane, and Qiskit

## Results
- Classical TGNN: 0.80 loss after 5 epochs
- Basic Q-TGNN: 0.66 loss after 5 epochs
- Enhanced Q-TGNN: 0.73 loss after 5 epochs

## Technologies Used
- PyTorch Geometric & Torch Geometric Temporal: For GNN modeling and handling temporal graph data.
- PennyLane: A quantum machine learning library for implementing and simulating quantum circuits.
- Qiskit: Used to build quantum circuits, specifically for QAOA layers in the enhanced Q-TGNN.
- Development Environment: Google Colab, utilizing available GPU resources to handle computational needs.

## Dataset
METR-LA traffic dataset (March 2012 - June 2012)
- 207 traffic sensors
- 12 timestep input/output windows
- Spatial-temporal traffic patterns

## Future Directions
Future work will focus on optimizing quantum layer configurations, exploring alternative quantum architectures, and testing Q-TGNNs in different domains like healthcare and finance. Access to more advanced quantum and GPU resources will further support the potential of Q-TGNNs for real-world traffic management.
