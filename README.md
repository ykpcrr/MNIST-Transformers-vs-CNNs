# CNN vs. Vision Transformer (ViT) Comparison on MNIST

In this project, I compared the performance of classical Deep Learning architectures (ResNet, VGG) and modern Vision Transformer (ViT) architecture on the MNIST dataset.

My goal was to test the "bigger the model, the better" perception on a relatively simple dataset and see the power of the Attention mechanism.

##  Models Used
The following models were tested under the same conditions:
1. **Custom Vision Transformer (ViT):** My own architecture using Multi-Head Attention.
2. **ResNet50 & ResNet101:** Transfer learning with ImageNet weights.
3. **VGG16:** Classic deep CNN architecture.

## 📊 Sonuçlar ve Karşılaştırma

| Model | Accuracy | Açıklama |
|-------|----------|----------|
| **ViT (Custom)** | **97.90%** | Highest performance and efficiency. |
| VGG16 | 97.16% | Best among CNN-based ones. |
| ResNet50 | 95.44% | Too complex for the dataset. |
| ResNet101 | 93.49% | Over-parameterization issue observed. |

##  Key Takeaways
* **ViT's Strength:** Without convolution layers, ViT achieved the highest success rate on this problem, using only patch and attention.
* **Complexity Balance:** Very deep models like ResNet101 struggled to learn on low-resolution data (28x28 -> 48x48 upscaled) like MNIST. It's been proven that "deeper isn't always better."

## 🛠 Teknolojiler
* **Framework:** TensorFlow / Keras
* **Language:** Python
* **techniques:** Transfer Learning, Data Augmentation, Multi-Head Attention Implementation.

---
*This project was developed by Yakup Acar.*
