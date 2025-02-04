---
title: "Deep Learning Course - Dementia Detection"
excerpt: "A deep-learning image classification model to address Alzheimer’s disease classification problem.<br/><br/><img src='/images/portfolio/brain_mri.jpg'><br/>"
collection: portfolio
---
**Project Grade**: 17/20

Complete project report [here](https://liveeduisegiunl-my.sharepoint.com/:b:/g/personal/20211652_novaims_unl_pt/EZ8l2xoPepFLnfgh9IRXywQBI7afnqvXevARYg7pBOUwyg?e=8XYogz)!

---

# Deep Learning for Alzheimer's Disease Classification: A Journey into Medical Image Analysis

As part of my academic journey in Deep Learning, I had the opportunity to work on a fascinating project that combines cutting-edge technology with healthcare applications. Together with my team, we developed a deep learning solution for classifying different stages of Alzheimer's disease using brain MRI scans.

## Project Overview

Alzheimer's disease represents one of the most significant challenges in modern healthcare. As our global population ages, the need for early and accurate diagnosis becomes increasingly crucial. Our project aimed to leverage the power of deep learning to assist in this diagnostic process by analyzing brain MRI scans.

Working with data from the Open Access Series of Imaging Studies, we developed a sophisticated 3D Convolutional Neural Network capable of distinguishing between four stages of cognitive function:
- Non Demented
- Very Mild Dementia
- Mild Dementia
- Moderate Dementia

## Technical Challenges and Innovations

One of the most interesting aspects of this project was developing a custom MRI selection algorithm. We needed to identify specific brain regions—particularly the temporal lobe and hypothalamus—as these areas show the earliest signs of Alzheimer's-related atrophy. Our algorithm automatically locates these crucial regions by identifying anatomical landmarks in the MRI scans.

The project involved several complex preprocessing steps:
- Intensity normalization to standardize MRI scan appearances
- Skull stripping to focus only on brain tissue
- Creation of consistent 3D image sequences for our neural network

Perhaps the most challenging aspect was dealing with variable MRI slice counts between patients. We solved this by developing an intelligent slice selection algorithm that ensures consistent input structure for our 3D CNN while maintaining focus on the most relevant brain regions.

## Results and Impact

Despite hardware limitations that restricted our batch sizes, our model achieved promising results:
- Weighted-average precision: 0.774
- Weighted-average recall: 0.785
- Weighted-average F1-score: 0.773

These metrics are particularly meaningful in the context of medical diagnosis, where false negatives could have serious consequences for patient care.

## Learning Outcomes

This project provided invaluable experience in:
- Medical image processing and analysis
- Deep learning architecture design
- Handling imbalanced datasets
- Working with 3D convolutional neural networks
- Developing custom preprocessing pipelines

The technical details, implementation challenges, and results are detailed in the full project report below.

---

*This project was completed as part of the Deep Learning course under Professors Mauro Castelli and Yuriy Perezhohin. Team members: Miguel Cardoso, Pedro Coimbras, Pedro Bonifácio, Petr Terletskiy, and Tiago Monteiro.*
