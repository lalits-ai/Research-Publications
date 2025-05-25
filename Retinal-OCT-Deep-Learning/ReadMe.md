## Abstract

Deep learning has emerged as a powerful tool in medical imaging, offering promising solutions for accurate and timely diagnosis of vision-threatening retinal disorders. This study compares four advanced deep learning architectures — **ResNet50**, **DenseNet121**, **Xception**, and **Vision Transformer (ViT)** — for the classification of **retinal Optical Coherence Tomography (OCT)** images into three pathological categories: **Choroidal Neovascularization (CNV)**, **Drusen**, and **Normal**.

Standard pre-processing and data augmentation techniques were applied to improve generalization, while training strategies like **early stopping**, **learning rate reduction on plateau**, and **class weighting** were used to counter overfitting and class imbalance.

### Key Findings:
- **ResNet50** achieved the highest classification accuracy at **92.13%**, showing strong reliability in detecting CNV cases.
- **DenseNet121** followed closely with **91.32%** accuracy.
- **Xception** and **ViT** also showed competitive performance, though slightly lower in comparison.
- **Confusion matrix analysis** validated ResNet50’s robustness, particularly in minimizing misclassifications of CNV images.

The models were implemented in **Python** using leading deep learning libraries like **TensorFlow**, **Keras**, and **PyTorch**, and were trained on **GPU-enabled systems**.

These results reinforce the effectiveness of **convolutional neural networks** in retinal image classification and highlight the **potential of transformer-based models** like ViT for further improvement. The comparative insights from this study provide valuable direction for developing **automated, robust diagnostic tools in ophthalmology**.

## Introduction

Deep learning algorithms combined with medical imaging have revolutionized automated diagnosis in recent years, particularly in **ophthalmology**. **Optical Coherence Tomography (OCT)** is a non-invasive imaging technique that produces high-resolution cross-sectional images of the retina, making it crucial for early detection and monitoring of retinal diseases.

Among the most prevalent retinal disorders are **Drusen** and **Choroidal Neovascularization (CNV)**, both of which can lead to partial or complete vision loss if left untreated. Manual diagnosis using OCT images is not only time-consuming but also subjective, emphasizing the need for **automated diagnostic systems** to assist clinicians in improving diagnostic speed and accuracy.

The objective of this project is to evaluate and compare the performance of several **state-of-the-art deep learning models** for classifying retinal OCT images into three categories: **Normal**, **Drusen**, and **CNV**. Specifically, this study focuses on four prominent architectures:
- **ResNet50**
- **DenseNet121**
- **Xception**
- **Vision Transformer (ViT)**

These models were selected based on their proven efficacy in computer vision tasks and their strong potential to enhance interpretation in medical imaging, especially for automated retinal disease diagnosis.

## Methodology and Motivation

To ensure robust performance, the OCT dataset was preprocessed using standard techniques including **normalization**, **resizing**, and **data augmentation**. These steps helped enhance generalization and prepare the data for efficient learning across all models.

Training optimization strategies such as:
- **Early Stopping**
- **Learning Rate Reduction on Plateau**
- **Class Weighting**

were employed to improve convergence and address **class imbalance** within the dataset.

Each model's performance was quantitatively evaluated using a comprehensive set of metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **Confusion Matrix**

The primary motivation for this study lies in the **growing global burden of preventable vision impairment** and the need for **AI-powered diagnostic systems** that are both scalable and reliable for deployment in real-world clinical settings.

By offering a comparative analysis of various deep learning architectures, this work aims to:
- Highlight each model’s **strengths and limitations**
- Provide insights for **future implementations** in medical image classification
- Encourage further research into **automated ophthalmic diagnostics**

## Results and Future Work

Based on the results obtained, **ResNet50** demonstrated the **best overall performance** among the evaluated models:

- **Accuracy:** 92.13%
- **Precision:** 92.21%
- **Recall:** 92.13%
- **F1-Score:** 92.12%

**DenseNet121** ranked a close second, delivering slightly lower but still robust performance. **Xception** also achieved competitive results, though marginally below ResNet50 and DenseNet121.

In contrast, the **Vision Transformer (ViT)** showed significantly lower performance, with all key metrics hovering around **71%**, suggesting it is currently less effective for this specific retinal OCT classification task.

These outcomes underscore the **superiority of CNN-based architectures** for medical imaging, especially when:
- The dataset size is relatively limited
- Fine-grained spatial feature extraction is critical
- Attention mechanisms in transformer models are not fully leveraged

### Key Takeaways:
- **ResNet50** is the most suitable architecture for retinal OCT classification.
- **DenseNet121** and **Xception** remain strong alternatives.
- Transformer-based models like **ViT** may require more data or architectural tuning.

### Future Work:
- Incorporate **Generative Adversarial Networks (GANs)** to augment the dataset and alleviate class imbalance.
- Explore advanced attention-based mechanisms and **transformer-CNN hybrids** for improved feature learning and generalization.

These directions aim to enhance the effectiveness of deep learning models in **automated retinal disease screening**, supporting scalable, accurate, and real-world clinical applications.
