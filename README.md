# Traditional-CV-vs-CNN
# Comparative Study on Object Recognition: Traditional Computer Vision vs. Deep Learning Approaches

This repository contains code and documentation related to a comparative study of object recognition techniques using traditional computer vision methods and deep learning approaches. The study focuses on analyzing the performance of Scale-Invariant Feature Transform (SIFT), Histogram of Oriented Gradients (HOG), and Convolutional Neural Networks (CNNs) on the CIFAR-10 dataset.

## Project Overview

In recent years, computer vision has become an essential component of robotics and AI, enabling machines to interpret and interact with the visual world. This project aims to compare the effectiveness of traditional feature extraction methods (SIFT and HOG) with modern deep learning techniques (CNNs) in object recognition tasks.

### Objectives
- Implement and evaluate SIFT and HOG as traditional computer vision methods for object recognition.
- Develop a CNN model to compare its performance against traditional methods.
- Analyze the strengths, weaknesses, and potential applications of each approach in the context of robotics.

## Methods

### Traditional Computer Vision

1. **SIFT (Scale-Invariant Feature Transform)**
   - Extracts distinctive features invariant to scale, rotation, and illumination.
   - Performance: ~30% accuracy on CIFAR-10.

2. **HOG (Histogram of Oriented Gradients)**
   - Focuses on gradient directions to capture edge, texture, and shape.
   - Performance: ~62% accuracy on CIFAR-10.

### Deep Learning Approach

- **CNN (Convolutional Neural Network)**
  - A multi-layered neural network designed to learn hierarchical features from data.
  - Architecture:
    - Convolutional layers with 32, 64, and 128 filters.
    - ReLU activations, MaxPooling, Dropout, Dense layers, and Softmax output.
  - Performance: ~82% accuracy on CIFAR-10.

## Results Summary

| Method | Accuracy | Precision | Recall | F1-Score |
|--------|----------|-----------|--------|----------|
| SIFT   | 30%      | 30%       | 30%    | 30%      |
| HOG    | 62%      | 62%       | 62%    | 62%      |
| CNN    | 82%      | 83%       | 82%    | 82%      |

### Key Insights

- **SIFT**: Effective for detecting invariant features but struggles with complex backgrounds and lower resolution images.
- **HOG**: Better captures edges and gradients, improving over SIFT, but still limited in noisy or featureless environments.
- **CNN**: Outperforms traditional methods significantly by learning complex patterns directly from the data, though it requires more computational resources.

## Discussion

The study highlights that while traditional methods like SIFT and HOG offer computationally efficient solutions, they fall short in accuracy compared to CNNs. CNNs, with their deep learning architecture, provide superior performance in complex image recognition tasks but at the cost of higher computational demands. The findings suggest a hybrid approach or further optimization of CNNs could benefit applications in robotics where both performance and efficiency are crucial.

## Usage

1. **Setup**: Clone the repository and install the necessary dependencies using the provided `requirements.txt`.
2. **Running Notebooks**: Execute the Jupyter Notebooks to replicate the experiments and analyze the results.
3. **Customization**: Modify the hyperparameters or model architecture in the notebooks to explore further optimizations.


Refer to the detailed [Report.pdf](./Report.pdf) for a complete list of references and an in-depth analysis of the methodologies used.

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
