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


# Results
![03a5ec87-ba7d-4845-bca7-c9c40eb7e05e](https://github.com/K-Hooshanfar/Chest-X-ray-Pneumonia-Detection-with-EfficientNet/assets/83825004/765d5891-ce1e-4d92-95ce-39d053b54609)

![4759f686-88fb-477a-ba1c-f419e7a8c82b](https://github.com/K-Hooshanfar/Chest-X-ray-Pneumonia-Detection-with-EfficientNet/assets/83825004/7872fcc2-fc15-48ac-afd9-6ea1d144c4e7)

![af346a58-0f3f-4572-a4c7-25d79db13492](https://github.com/K-Hooshanfar/Chest-X-ray-Pneumonia-Detection-with-EfficientNet/assets/83825004/7447099a-173c-438e-aec3-7b2fc2c9d312)




