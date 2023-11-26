# Deep-Cross-Network-DCN
DCN was designed to learn explicit and bounded-degree cross features more effectively. It starts with an input layer (typically an embedding layer), followed by a cross network containing multiple cross layers that models explicit feature interactions, and then combines with a deep network that models implicit feature interactions.

---
 
## Overview
 
The Deep & Cross Network (DCN) is designed to effectively learn explicit and bounded-degree cross features within data, especially in scenarios where feature interactions play a crucial role.
 
### Feature Crosses
 
Feature crosses represent the combined interaction of individual features. In the context of a recommender system, such crosses can signify important connections that drive user behavior.
 
![Feature Crosses](http://drive.google.com/uc?export=view&id=1e8pYZHM1ZSwqBLYVkKDoGg0_2t2UPc2y)
 
### Challenges and DCN's Solution
 
The challenges in learning feature crosses often arise from large and sparse categorical data. DCN addresses this by utilizing both a Cross Network and a Deep Network.
 
### DCN Architecture
 
#### Cross Network
The core of DCN, it explicitly models feature crosses at each layer, increasing the polynomial degree with layer depth.
 
![Cross Network](http://drive.google.com/uc?export=view&id=1QvIDptMxixFNp6P4bBqMN4AYAhAIAYQZ)
 
#### Deep Network
A traditional feedforward multilayer perceptron (MLP).
 
![Deep Network](http://drive.google.com/uc?export=view&id=1WtDUCV6b-eetUnWVCAmcPh8mJFut5EUd)
 
## Usage
 
### Toy Example
 
Illustrates the benefits of DCN using a simple dataset.
 
### Movielens 1M Example
 
Demonstrates DCN's effectiveness on real-world data from the Movielens 1M dataset.
 
## Code Structure
 
The code is structured into several sections:
 
- **Synthetic Data Generation**: Illustrates data creation following a specific distribution.
- **Model Construction**: Defines the DCN model and a unified model class for loss computation.
- **Model Training**: Details the process of preparing, compiling, and training the DCN models.
- **Model Evaluation**: Evaluates and compares the performance of DCN and other models.
- **Model Understanding**: Visualizes the learned weight matrix in DCN to understand important feature crosses.
 
## Getting Started
 
To use this code, follow these steps:
 
1. Install necessary packages using `pip install`.
2. Run the code sections sequentially in your preferred environment.
 
## Results
 
The evaluation of DCN's performance on both toy and real-world datasets is detailed, showcasing its superiority over traditional DNNs.
 
## Further Possibilities
 
Explore additional ways to utilize DCN, such as parallel structures or concatenated cross layers.
