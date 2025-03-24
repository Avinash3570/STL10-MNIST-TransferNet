**Transfer Learning in PyTorch: STL-10 to MNIST**

**📌 Project Overview**

This project demonstrates **transfer learning** using PyTorch by pre-training a **Convolutional Neural Network (CNN)** on the **STL-10** dataset and adapting it to the **MNIST** dataset. The goal is to leverage knowledge learned from a large dataset and effectively transfer it to a smaller, domain-specific dataset.

**🚀 Implementation Steps**

1. **Preprocess both datasets**
   1. Normalize, resize, and augment images.
   1. Set up PyTorch DataLoaders for training and validation.
1. **Pre-train a CNN on STL-10**
   1. Train a model from scratch or use a pre-trained model trained only on STL-10.
   1. Log training metrics such as loss and accuracy.
1. **Transfer learning on MNIST**
   1. **Approach 1**: Train only the linear (fully connected) layers while keeping convolutional layers frozen.
   1. **Approach 2**: Freeze the initial few layers of the feature extractor and train others.
   1. **Approach 3**: Fine-tune the entire network.
1. **Evaluate the adapted model on MNIST**
   1. Compute **overall accuracy** and per-class **precision, recall, F1-score**.
   1. Generate and analyze **confusion matrices**.

**📊 Datasets Used**

- [**STL-10**](https://cs.stanford.edu/~acoates/stl10/): 10-class dataset with 96×96 RGB images.
- **MNIST**: Handwritten digit dataset with 28×28 grayscale images.

**🛠 Technologies Used**

- **Python**
- **PyTorch**
- **Torchvision**
- **Matplotlib & Seaborn** (for visualization)

**📌 Results & Insights**

- Performance comparison across different transfer learning strategies.
- Impact of freezing different layers on model generalization.
- Visualization of misclassified samples using confusion matrices.

