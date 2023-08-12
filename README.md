# Chest-X-ray-Pneumonia-Detection-with-EfficientNet

This repository contains implementation of "Automated Diagnosis of Pneumonia from Chest X-Ray Images using EfficientNet". You can find the article here:[IEEE](https://ieeexplore.ieee.org/document/9397055)

# Dataset

The dataset, comprising a total of 5,863 X-ray images, can be found [here](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia). It includes:

* 4,273 pneumonia images

* 1,583 normal images

Given the limited data, especially in the validation set, a consolidation approach has been employed. All pneumonia images have been combined into a single dataset, and likewise, all normal images are grouped in another dataset. Subsequently, the data is divided into the following splits:

- Training dataset: 60% of the data (950 normal images, 2,563 pneumonia images)

- Validation dataset: 20% of the data (317 normal images, 855 pneumonia images)

- Testing dataset: 20% of the data (316 normal images, 855 pneumonia images)

But the dataset is still imbalanced by a varying amount of Pneumonia/Normal images for each collection. To reduce this issue, the paper suggests that we use ’CLASS WEIGHTS’ parameter.
 
# Data Preprocessing and Augmentation

Due to data limitations, data augmentation techniques have been employed to address this issue while also reduce overfitting. Resizing images to 128x128 dimensions is performed as a preprocessing step. This process enhances data diversity and aids model generalization. Various techniques have been used for data augmentation, as summarized below:

Horizontal Flipping - Rotation - Zooming - Brightness Adjustment - Shearing


# Dataset
