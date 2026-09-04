# Enhancing the Identification of Brain Tumours Using the CNN Ensemble Model

**Paper:** https://doi.org/10.56532/mjsat.v4i3.264

Abstract
The early and accurate detection of brain tumors is a critical challenge in diagnostics and healthcare due to the severe consequences of delayed diagnosis. This paper addresses this issue by employing an ensemble of Convolutional Neural Network (CNN) models to enhance the identification of brain tumors using MRI images. The methodology integrates pre-processing techniques such as image augmentation, Gaussian blurring, and Sobel edge detection to improve image quality. Various CNN architectures, including Scratch CNN, InceptionV3, Xception, EfficientNetB0, ResNet50, and VGG19, were evaluated alongside machine learning classifiers such as AdaBoost, Random Forest, SVM, KNN, and SoftMax. Among these, EfficientNetB0, Xception, and InceptionV3 demonstrated superior performance, achieving the highest classification accuracy of 98.67% and an average accuracy of 96.90%. This research underscores the significance of selecting appropriate models and classifiers for medical image classification and highlights the potential for further advancements in clinical applications.



This repository contains the implementation and experimental work for the research paper **“Enhancing the Identification of Brain Tumours Using the CNN Ensemble Model,”** published in the *Malaysian Journal of Science and Advanced Technology*, Volume 4, Issue 3, pp. 338–353, 2024.


## Methodology

The experimental workflow consists of:

1. **MRI Image Preprocessing**

   * Image augmentation
   * Gaussian blurring
   * Sobel edge detection
   * Image preparation for CNN-based feature extraction

2. **CNN Feature Extraction**

   Several CNN architectures were investigated:

   * Custom/Scratch CNN
   * InceptionV3
   * Xception
   * EfficientNetB0
   * ResNet50
   * VGG19

3. **Machine Learning Classification**

   Features extracted from the CNN models were evaluated using:

   * AdaBoost
   * Random Forest
   * Support Vector Machine (SVM)
   * K-Nearest Neighbors (KNN)
   * Softmax

4. **CNN Ensemble Experiments**

   Multiple CNN feature combinations were investigated, including:

   * InceptionV3 + EfficientNetB0
   * EfficientNetB0 + Xception
   * InceptionV3 + Xception
   * Multi-model combinations

5. **Performance Evaluation**

   The models were compared using classification accuracy and log loss to identify the most effective architectures and combinations.

## Results

Among the individual CNN architectures, **EfficientNetB0 achieved the strongest average performance**, with an average accuracy of approximately **97.87%** in the repository experiments.

The ensemble experiments further demonstrated the effectiveness of combining complementary CNN feature representations. The best reported ensemble configuration achieved an **average accuracy of 96.90%**, while the research reported a maximum classification accuracy of **98.67%**.

These results demonstrate the potential of combining deep CNN-based feature extraction with traditional machine learning classifiers for MRI-based brain tumour identification.

## Repository Structure

```text
THESIS-G56/
│
├── Final Code/
│   ├── Thesis.ipynb
│   ├── Code base interface and graph.ipynb
│   ├── Brain MRI.zip
│   ├── PICTURES/
│   ├── PICTURES.zip
│   ├── Note.txt
│   └── Proccess.txt
│
├── Main Paper/
│   └── Research paper
│
├── OLD/
│   └── Previous experiments and development files
│
└── README.md
```

## Dataset

The experiments use the **Brain Tumor Detection dataset (Br35H)** containing MRI images for brain tumour detection.

Dataset source:

https://www.kaggle.com/datasets/ahmedhamada0/brain-tumor-detection

## Technologies

* Python
* TensorFlow
* Keras
* Scikit-learn
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Jupyter Notebook

## Key Contributions

* Investigated multiple CNN architectures for MRI-based brain tumour identification.
* Applied image preprocessing and augmentation techniques to improve image representation.
* Compared CNN-derived features using multiple machine learning classifiers.
* Evaluated individual CNN architectures and CNN ensemble combinations.
* Compared models using both accuracy and log-loss metrics.
* Identified high-performing CNN and classifier combinations for the investigated dataset.

## Publication

**Mohi Uddin Anando, Rabbi Hasan Himel, and Shifar Tanjam.**

*Enhancing the Identification of Brain Tumours Using the CNN Ensemble Model.*

**Malaysian Journal of Science and Advanced Technology**, Vol. 4, Issue 3, pp. 338–353, 2024.

DOI: https://doi.org/10.56532/mjsat.v4i3.264

Published: August 2024.

## Citation

```bibtex
@article{anando2024enhancing,
  title={Enhancing the Identification of Brain Tumours Using the CNN Ensemble Model},
  author={Anando, Mohi Uddin and Himel, Rabbi Hasan and Tanjam, Shifar},
  journal={Malaysian Journal of Science and Advanced Technology},
  volume={4},
  number={3},
  pages={338--353},
  year={2024},
  doi={10.56532/mjsat.v4i3.264}
}
```

## Disclaimer

This project is a research implementation intended for experimentation and academic purposes. The reported results are specific to the dataset, preprocessing pipeline, architectures, classifiers, and experimental configuration used in the study. The system should not be considered a clinically validated diagnostic tool.
