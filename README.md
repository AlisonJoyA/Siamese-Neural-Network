# Siamese-Neural-Network
# Optical Fibre Sensing Signal Recognition Based on Siamese Neural Network

## Overview
Distributed fibre optic sensing technology has applications in fields such as pipeline safety and perimeter defence. However, vibration sensing signals often contain significant noise and stray signals, leading to false alarms. To enhance the accuracy of pre-warnings, it is crucial to accurately identify signal types.

## Motivation
Deep learning models like Convolutional Neural Networks (CNN) improve vibration sensing event recognition in Φ-OTDR (Phase-sensitive Optical Time Domain Reflectometry) systems. However, training such models requires large datasets, which are often limited in the case of Φ-OTDR event recognition. This limitation makes it challenging to effectively train neural networks for signal classification.

## Proposed Approach
This project explores the use of **Siamese Neural Networks (SNN)** for optical fibre sensing signal recognition. A dataset consisting of **400 time-frequency diagram samples** from a publicly available dataset released by researchers at Zhejiang University was used to train and evaluate two models:
1. A **16-layer Visual Geometry Group (VGG-16) neural network**
2. A **Siamese Neural Network (SNN) based on VGG-16**

## Performance Comparison
| Model | Accuracy | Signal Recognition Accuracy |
|-------|-----------|--------------------------|
| **VGG-16** | 17.50% | - |
| **SNN (VGG-16 based)** | 90.62% | 90.0% |

### Key Findings
- The **Siamese Neural Network significantly outperforms the VGG-16 model**, especially in scenarios with limited training data.
- SNNs can improve optical fibre sensing signal recognition, making them a viable approach for real-world applications where large datasets are unavailable.

## Repository Structure
```
📂 Project Root
 ├── 📁 data                 # Dataset (time-frequency diagrams)
 ├── 📁 models               # Trained model architectures
 ├── 📁 scripts              # Training and evaluation scripts
 ├── 📄 README.md            # Project documentation
 ├── 📄 requirements.txt      # Dependencies
```



## Conclusion
This project demonstrates the effectiveness of **Siamese Neural Networks for vibration signal recognition in optical fibre sensing**. Future work includes expanding the dataset, fine-tuning hyperparameters, and exploring real-time applications of this technology.

---
### Citation
This project uses original dataset from Zhejiang University. I am currently unable to publish the code as this research is still under review. I will update this respiratory as soon as I can

---
**Author:** [Alison Joy]  
**Acknowledgment:** Zhejiang University for providing the dataset
