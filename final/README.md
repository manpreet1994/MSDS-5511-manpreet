Street Food Image Classification

Overview
This project explores the performance of various deep learning architectures for an image classification task. It compares Convolutional Neural Networks (CNNs), Vision Transformers (ViT) with and without self-attention, ResNet, and EfficientNet models.

Key Findings
The standard Convolutional Neural Network (CNN) demonstrated the best performance, achieving a training accuracy of 0.857877, validation accuracy of 0.318801, and validation top-3 accuracy of 0.591281.

The self-attention Vision Transformer (ViT) model showed the second-best performance across all metrics, suggesting the potential benefits of attention mechanisms in vision transformers. However, it still lagged considerably behind the CNN.

EfficientNet and vanilla ViT models exhibited the lowest performance, indicating their current configurations or inherent architectures were less suitable for this specific image classification task compared to CNNs or self-attention ViTs.

ResNet also underperformed relative to the CNN and self-attention ViT.

Discussion and Limitations
The strong performance of the CNN highlights its applicability for this particular classification problem. A major reason for the CNN's superior performance could be the limited size of the dataset; each of the 20 image labels had only 150-200 images. Vision Transformers are known to be "data hungry," and this exercise reinforces that characteristic. For large, complex CNNs like ResNet and EfficientNet, their massive capacity (depth and number of parameters) can lead to overfitting on very small datasets without careful regularization or transfer learning.

Conclusion
Further optimization or different architectural choices may be needed for the transformer and other models to reach comparable performance to CNNs on this specific image classification task, especially with smaller datasets.