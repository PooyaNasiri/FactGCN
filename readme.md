# FastGCN and Enhanced Sampling Techniques

## Overview
This project focuses on implementing FastGCN, a scalable alternative to traditional Graph Convolutional Networks (GCNs) that leverages importance sampling to improve efficiency. Additionally, we explore adaptive sampling techniques to further enhance accuracy and computational performance.

## Authors
- Pooya Nasiri (pooya.nasiri@studenti.unipd.it)
- Giacomo Vettoretti (giacomo.vettoretti@studenti.unipd.it)
- Jacopo Righetto (jacopo.righetto@studenti.unipd.it)

## Features
- Implementation of FastGCN with importance sampling
- Adaptive sampling strategy to improve accuracy
- Comparative analysis with traditional GCNs
- Experiments conducted on benchmark datasets: MNIST, Cora, PubMed, CiteSeer
- Performance evaluation based on training time, accuracy, and memory usage

## Installation
To run the project, install the necessary dependencies:

```sh
pip install torch torchvision numpy scipy scikit-learn matplotlib
```

## Usage
The project is implemented in Jupyter Notebook. To run the notebook:

```sh
jupyter notebook FastGCN.ipynb
```

### Running Experiments
1. Load the dataset (MNIST, Cora, PubMed, or CiteSeer)
2. Preprocess the graph data (adjacency matrix, feature normalization)
3. Train FastGCN using the implemented model
4. Evaluate results using classification accuracy and computational efficiency

## Datasets
- **MNIST**: Converted into a graph format where nodes represent images.
- **Cora**: Citation network of scientific publications categorized into seven classes.
- **PubMed**: Biomedical articles classified into three categories.
- **CiteSeer**: Research paper citation network with six categories.

## Results
- **FastGCN reduces training time** compared to traditional GCNs.
- **Adaptive sampling improves accuracy** by selecting influential nodes dynamically.
- **Trade-off observed between efficiency and accuracy**, with importance sampling optimizing computational cost.
- **Dataset-specific tuning** is crucial for achieving optimal performance.

### Test Accuracies with Adaptive Sampling
| Dataset  | Test Accuracy |
|----------|--------------|
| MNIST    | 0.2500       |
| PubMed   | 0.5000       |
| Cora     | 0.1407       |
| CiteSeer | 0.2218       |

## Future Work
- Exploring **hybrid sampling techniques** combining multiple strategies.
- Fine-tuning **importance sampling distributions** for different datasets.
- Implementing **hierarchical sampling** for large-scale graphs.
- Integrating **adaptive learning rates** for better convergence.

## References
- Jie Chen, Tengfei Ma, and Cao Xiao. FastGCN: Fast learning with graph convolutional networks via importance sampling (ICLR, 2018).
- William L. Hamilton, Rex Ying, and Jure Leskovec. Inductive representation learning on large graphs (2018).
- Thomas N. Kipf and Max Welling. Semi-supervised classification with graph convolutional networks (2017).
