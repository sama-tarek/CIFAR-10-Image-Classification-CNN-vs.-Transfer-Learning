# CIFAR-10 Image Classification: CNN vs. Transfer Learning

## 📌 Project Overview

This project explores image classification using Deep Learning by comparing a **Convolutional Neural Network (CNN) built from scratch** with **Transfer Learning using a pretrained model** on the CIFAR-10 dataset.

The goal is to evaluate how different architectures learn visual features and classify images into multiple categories, comparing their predictive performance and training behavior.

## 🎯 Objectives

- Build and train a CNN from scratch for image classification.
- Apply Transfer Learning using a pretrained model.
- Perform fine-tuning to improve classification performance.
- Evaluate models using multiple classification metrics.
- Compare model performance to understand the benefits of pretrained feature extraction.

## 📂 Dataset

The project uses the **CIFAR-10 dataset**, a benchmark dataset containing 60,000 color images across 10 classes.

- **Training images:** 50,000
- **Test images:** 10,000
- **Image dimensions:** 32 × 32 pixels
- **Number of classes:** 10
- **Image format:** RGB

### Classes

Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, and Truck.

## 🛠️ Technologies & Libraries

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 🧠 Methodology

### 1. Data Preparation
- Load and inspect the CIFAR-10 dataset.
- Normalize image pixel values.
- Prepare training, validation, and test datasets.
- Apply the preprocessing required by the selected architectures.

### 2. CNN From Scratch
- Build a custom CNN architecture using convolutional and pooling layers.
- Train the model to learn image features directly from the dataset.
- Monitor training and validation performance.
- Evaluate classification results on the test set.

### 3. Transfer Learning
- Use a pretrained deep learning model as a feature extractor.
- Adapt the classification head to the 10 CIFAR-10 classes.
- Train the new classification layers.
- Fine-tune selected layers of the pretrained model to adapt learned features to the target dataset.

### 4. Model Evaluation
Evaluate model performance using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Training and validation curves

### 5. Performance Comparison
Compare the CNN and Transfer Learning approaches based on:
- Classification performance
- Generalization on unseen images
- Training behavior
- Per-class performance

## 📊 Results & Model Comparison

All models were evaluated on the CIFAR-10 test set containing 10,000 images.

| Model | Test Accuracy | Test Loss |
|---|---:|---:|
| Custom CNN (From Scratch) | 72.86% | 0.7789 |
| MobileNetV2 (Feature Extraction) | 84.99% | 0.4445 |
| MobileNetV2 (Fine-Tuned) | **92.66%** | **0.2292** |

### Key Findings

- **Custom CNN:** Achieved 72.86% test accuracy by learning image features directly from the CIFAR-10 dataset.
- **Transfer Learning:** MobileNetV2 improved test accuracy to 84.99% by leveraging pretrained visual features.
- **Fine-Tuning:** Fine-tuning MobileNetV2 achieved the best result, with **92.66% test accuracy** and a test loss of 0.2292.

### Conclusion

Transfer Learning significantly improved image classification performance compared with the custom CNN. Fine-tuning the pretrained MobileNetV2 model delivered the strongest results, demonstrating the value of adapting pretrained visual representations to the target dataset.

## 📁 Project Structure

```text
CIFAR-10-Image-Classification/
│
├── notebooks/
│   └── CIFAR-10_Deep_Learning.ipynb
│
├── README.md
└── requirements.txt
```

*Adjust the structure to match the actual files in your repository.*

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/sama-tarek/CIFAR-10-Image-Classification.git
cd CIFAR-10-Image-Classification
```

### 2. Install Dependencies

```bash
pip install tensorflow numpy matplotlib scikit-learn jupyter
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebooks and run the cells sequentially.

The CIFAR-10 dataset can be loaded directly through TensorFlow/Keras, so a separate manual download may not be necessary.

## 💡 Key Learnings

- Understanding CNN architectures and image feature extraction.
- Implementing multi-class image classification.
- Applying Transfer Learning and fine-tuning.
- Monitoring overfitting and generalization.
- Evaluating models using class-level metrics.
- Comparing custom architectures with pretrained deep learning models.

## 👩‍💻 Author

**Sama Tarek**

AI Student | Data Science & Machine Learning Enthusiast

- **GitHub:** [sama-tarek](https://github.com/sama-tarek)
- **LinkedIn:** [Sama Tarek](https://www.linkedin.com/in/sama-tarek-757536249/)
- **Email:** samatarek1711@gmail.com

---

⭐ If you find this project interesting, feel free to explore the notebooks and review the model comparisons.
