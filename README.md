# vehicle_classification_model-utd
A custom Convolutional Neural Network (CNN) built from scratch for robust vehicle perception in autonomous systems. This project achieves 78.54% test accuracy across 8 classes using a safety-first architecture (Batch Normalization &amp; Dropout) to ensure high generalization and reliable real-world performance.

# 🏎️ Vehicle Classification Model - UTD
A high-performance Convolutional Neural Network (CNN). This project evaluates model robustness and generalization in autonomous perception tasks.

## 📊 Current Status
* **Test Accuracy:** 78.54% (Target: >50%)
* **Generalization Gap:** <0.1% (Stable alignment between Train/Test)
* **Demo:** [Live on Hugging Face Spaces]((https://huggingface.co/spaces/abhiprd20/vehicle_classification_model-utd))

## 🏗️ Model Architecture
A custom-built CNN designed for transparency and interpretability in feature extraction:
* **Feature Extractor:** 3-stage Convolutional blocks (16, 32, 64 filters).
* **Safety Regularization:** Integrated **Dropout (0.5)** and **BatchNorm2d** after every convolution to ensure the model learns redundant, robust features rather than memorizing dataset artifacts.
* **Classifier:** Dual-layer MLP with Cross-Entropy Loss optimization.

## 📂 Dataset Details
* **Images:** 26,378 categorized vehicle images.
* **Classes:** 8 (Bicycle, Bus, Car, Motorcycle, NonVehicles, Taxi, Truck, Van).
* **Split:** Strict 8:2 ratio (21,102 training / 5,276 testing).
* **Preprocessing:** Standardized 224x224 input with ImageNet-standard normalization.

## 🛡️ AI Safety & Error Analysis
* **Critical Detection:** Near-zero false-negative rate for `NonVehicles` (1,775/1,800 correct), essential for avoiding "ghost braking" in autonomous systems.
* **Edge Case Identification:** Confusion matrix reveals geometric similarities between `Bicycle` and `Motorcycle`, identifying a specific area for future fine-tuning.

## 📚 Research & Development Portfolio
*This project is part of my broader commitment to AI and Computer Science research.*

## 🛠️ Key Projects
* **Bhojpuri Language Dataset**: Curated and published 100k+ rows datasets on Hugging Face for regional NLP research.
* **CNSD Model Architecture**: Authored research on neural network configurations for optimized feature extraction.
* Custom 4 sentiment models, 1 vehicle classification model and several datasets.
* Link to my Hugging Face account : https://huggingface.co/abhiprd20 (with all models and datasets)
* E-mail : abhiprd20@gmail.com
* My research paper pre-print : https://zenodo.org/records/19054785
* 2nd research project : https://github.com/abhiprd200/CNSD_prototype
* My github with other projects : https://github.com/abhiprd200

## Contact
* E-mail : abhiprd20@gmail.com
---
**License:** Apache 2.0
