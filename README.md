# Detection of Melanoma Skin Cancer

## Abstract
In the realm of cancer, there exist more than 200 distinct forms, with melanoma standing out as the most lethal form of skin cancer. The diagnostic journey for melanoma initiates with clinical screening, followed by dermoscopic analysis and histopathological examination. Early identification of melanoma skin cancer significantly enhances the chances of successful treatment. The initial stage involves visually examining the affected skin area, capturing dermatoscopic images through a high-speed camera. These images boast an accuracy of 65-80% in melanoma diagnosis without additional technical support. Further scrutiny by cancer treatment specialists, combined with dermatoscopic images, elevates the overall prediction accuracy to 75-84%. This project endeavors to construct an automated classification system using image processing techniques to identify skin cancer based on skin lesion images.

## Problem Statement
During a skin biopsy, dermatologists extract a portion of the skin lesion for microscopic examination. The current process, from scheduling a dermatologist appointment to receiving a biopsy report, spans almost a week or more. The objective is to narrow this timeframe to just a couple of days through the implementation of a predictive model. The proposed approach utilizes a Convolutional Neural Network (CNN) to classify nine types of skin cancer from outlier lesion images. This reduction in processing time has the potential to positively impact millions of people.

## Motivation
The overarching objective is to contribute to the reduction of deaths caused by skin cancer. The driving force behind this project is the utilization of advanced image classification technology for the betterment of people's well-being. The progress made in computer vision, machine learning, and deep learning has paved the way for scalable applications across various domains.

## Dataset
The dataset comprises 2357 images of malignant and benign oncological diseases sourced from the International Skin Imaging Collaboration (ISIC). These images were categorized based on the ISIC classification, with each subset containing an equal number of images. To address class imbalance, the Python package Augmentor (https://augmentor.readthedocs.io/en/master/) was employed to augment samples across all classes, ensuring a balanced representation.

## CNN Architecture Design
A custom CNN model was developed to classify skin cancer using skin lesion images, aiming for heightened accuracy and task performance. The architectural elements include:

- Rescaling Layer: Converts input from the [0, 255] range to [0, 1].
- Convolutional Layer: Applies convolution operation, condensing information in receptive fields.
- Pooling Layer: Reduces feature map dimensions, minimizing parameters and computation.
- Dropout Layer: Prevents overfitting by randomly setting input units to zero during training.
- Flatten Layer: Converts output into a 1-dimensional array for the next layer.
- Dense Layer: Deeply connected neural network layer, receiving input from the preceding layer.
- Activation Function (ReLU): Piecewise linear function addressing the vanishing gradient problem.

## References
- Melanoma Skin Cancer: https://www.cancer.org/cancer/melanoma-skin-cancer/about/what-is-melanoma.html
- Introduction to CNN: https://www.analyticsvidhya.com/blog/2021/05/convolutional-neural-networks-cnn/
- Image Classification using CNN: https://www.analyticsvidhya.com/blog/2020/02/learn-image-classification-cnn-convolutional-neural-networks-3-datasets/
- Efficient CNN Architecture: https://towardsdatascience.com/a-guide-to-an-efficient-way-to-build-neural-network-architectures-part-ii-hyper-parameter-42efca01e5d7
