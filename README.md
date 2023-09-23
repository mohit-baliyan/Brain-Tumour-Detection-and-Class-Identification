# Brain-Tumour-Detection-and-Class-Identification
# Project Title: Brain Tumor Detection and Classification

## Abstract
The National Cancer Institute reports that approximately 24,530 patients were diagnosed with brain cancer in the United States in 2021, with a 5-year survival rate of around 32.6%. Accurate and early detection of brain tumors is crucial for improving patient outcomes. Currently, the gold standard for brain tumor diagnosis relies on radiologists' interpretation of Magnetic Resonance Imaging (MRI) scans, which can be subject to human error. To address this issue, we have developed a solution using Convolutional Neural Networks (CNNs) to identify three types of brain tumors—gliomas, meningiomas, and pituitary tumors. This project explores various CNN approaches to classify these tumors and demonstrates the effectiveness of ensemble techniques in achieving highly accurate results.

**GitHub Repository**: [Link to Code](#insert-link-here)

## Introduction

### Background
Brain tumors can exert pressure on surrounding tissues, leading to symptoms such as headaches, nausea, and balance problems. This project focuses on the detection and classification of three major types of brain tumors:

1. **Gliomas:** These tumors originate in the glial cells surrounding nerves and are most common in adults aged 45 to 65. Symptoms include headaches, memory loss, speech problems, and seizures.

   ![Glioma](insert-image-link-here)

2. **Meningiomas:** Meningiomas are the most common brain tumors, arising in the membranes surrounding the brain and spinal cord. Symptoms may include vision changes, headaches, hearing loss, and language difficulties.

   ![Meningioma](insert-image-link-here)

3. **Pituitary Tumors:** These tumors develop in the pituitary gland, affecting hormone production. Symptoms include headaches, peripheral vision loss, weight changes, increased urination, weakness, and sexual dysfunction.

   ![Pituitary Tumor](insert-image-link-here)

### Problem Statement
Radiologist interpretation of MRI scans for brain tumor diagnosis can be costly, time-consuming, and prone to errors. Our project aims to address these challenges:

1. **Augment Radiologist Abilities:** Develop a model to quickly detect brain tumors and identify their types, aiding radiologists in devising treatment plans and prioritizing patients.

2. **Improve Affordability:** Help patients avoid unnecessary radiologist appointments and consultation fees when no tumor is detected.

## Related Work
Prior research in brain tumor segmentation using CNNs has gained popularity. A 2019 study achieved a 3-class classification problem similar to our project, achieving 98% accuracy using transfer learning [4]. Additionally, techniques like image augmentation, as demonstrated in a study by Sajjad [5], were incorporated into our data pre-processing.

## Approach Outline and Novel Characteristics
Our research focuses on evaluating different neural network techniques for classifying brain tumor images, including:

1. **CNN:** A model with 3 convolutional layers and 2 feed-forward layers.

2. **VGG-16:** Transfer learning with VGG-16 architecture.

3. **RESNET-152:** Transfer learning with RESNET-152 architecture.

4. **Inception V3:** Transfer learning with Inception V3 architecture.

Transfer learning involved retraining the final layers of the models to enhance accuracy. Ensemble techniques were applied to combine model outputs for improved performance.

## Data Description
We utilized a Kaggle dataset for training and evaluation, containing 4 distinct classes: Glioma, Meningioma, Pituitary Tumor, and No Tumor. The dataset comprises 5,712 images in the training set and 1,311 images in the test set.

### Data Pre-processing Techniques
Our data pre-processing involved:

- Standardizing Image Resolutions to 224x224 px for compatibility with transfer learning.
- Image Augmentation to maintain spatial data and increase the dataset size.

```python
# Code Snippet for Data Augmentation
insert-code-snippet-here
