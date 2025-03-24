# ﻿**Transfer Learning in PyTorch: STL-10 to MNIST**

# **📌 Project Overview**

This project demonstrates **transfer learning** using PyTorch by pre-training a **Convolutional Neural Network (CNN)** on the **STL-10** dataset and adapting it to the **MNIST** dataset. The goal is to leverage knowledge learned from a large dataset and effectively transfer it to a smaller, domain-specific dataset.

# **🚀 Implementation Steps**

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

# **📊 Datasets Used**

- [**STL-10**](https://cs.stanford.edu/~acoates/stl10/): 10-class dataset with 96×96 RGB images.
- **MNIST**: Handwritten digit dataset with 28×28 grayscale images.

# **🛠 Technologies Used**

- **Python**
- **PyTorch**
- **Torchvision**
- **Matplotlib & Seaborn** (for visualization)

# **📌 Results & Insights**

- Performance comparison across different transfer learning strategies.
- Impact of freezing different layers on model generalization.
- Visualization of misclassified samples using confusion matrices.


![8](https://github.com/user-attachments/assets/4d561e68-ebc3-4263-bd49-23a37f955b4c)
![7](https://github.com/user-attachments/assets/d829ce55-c7d6-442e-bf3a-3026a80a65d3)
![6](https://github.com/user-attachments/assets/99e026be-d2c7-4567-a243-c8b3098681c8)
![5](https://github.com/user-attachments/assets/b33ac39e-d010-4510-a692-cbb1c91f8fc1)
![4](https://github.com/user-attachments/assets/83dffe46-5183-4419-a2a3-1073caa06760)
![3](https://github.com/user-attachments/assets/e6c2f125-d600-439e-838b-474c4e4423f6)
![2](https://github.com/user-attachments/assets/ad2f0d20-244a-4d18-bfea-d9b9440e6caf)
![1](https://github.com/user-attachments/assets/6f6e54c8-adbf-4267-9888-2c95b1e07216)
