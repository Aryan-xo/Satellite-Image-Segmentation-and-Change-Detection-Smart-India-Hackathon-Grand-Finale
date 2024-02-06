# Change Detection due to Human Activities

## Overview

This project aims to develop an automated system for detecting changes related only to human activities using satellite imagery. Specifically, the goal is to create an AI/ML-based model capable of detecting changes in man-made objects such as vehicles, buildings, roads, aircraft, etc., from remote sensing images. The primary datasets used for this task are Sentinel-2 and LISS-4.

## Model Development

### Data Collection and Preprocessing

Satellite imagery data from the Sentinel-2 and LISS-4 datasets is collected and preprocessed for model training. The images are resized, normalized, and segmented into patches to prepare them for input into the model.

### Model Architecture

The model architecture is based on a modified U-Net architecture, optimized for semantic segmentation tasks. It consists of convolutional layers with dropout regularization, followed by transposed convolutional layers for upsampling. The final layer uses softmax activation to output pixel-wise probability distributions over different classes of man-made objects.

### Training and Evaluation

The model is trained using a combination of Dice loss and Focal loss as the loss function, optimized using the Adam optimizer. Training is performed on a subset of the dataset, while the performance is evaluated using validation data. Metrics such as accuracy and Jaccard coefficient (IoU) are used to assess the model's performance.

## Results

The trained model demonstrates promising results in detecting changes related to human activities from satellite imagery. Visualizations comparing original images, ground truth masks, and predicted masks show the model's ability to accurately identify man-made objects in the images.

### Example Images

![Training Data](https://github.com/Aryan-xo/Satellite-Image-Segmentation-and-Change-Detection-Smart-India-Hackathon-Grand-Finale/blob/main/loss.png?raw=true)

![Prediction_1](https://github.com/Aryan-xo/Satellite-Image-Segmentation-and-Change-Detection-Smart-India-Hackathon-Grand-Finale/blob/main/Prediction.png?raw=true)

![Prediction_2](https://github.com/Aryan-xo/Satellite-Image-Segmentation-and-Change-Detection-Smart-India-Hackathon-Grand-Finale/blob/main/Prediction2.png?raw=true))

## Conclusion

This project showcases the potential of AI/ML techniques in automating change detection tasks from satellite imagery, specifically focusing on human-related activities. By accurately detecting changes in man-made objects, this system can be valuable for various applications such as urban planning, environmental monitoring, and disaster response.
