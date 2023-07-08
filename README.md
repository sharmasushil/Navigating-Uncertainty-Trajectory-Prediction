# Navigating Uncertainty: The Role of Short-Term Trajectory Prediction in Autonomous Vehicle Safety 🚘
Abstract: Autonomous vehicles require accurate and reliable short-term trajectory predictions for safe and efficient driving. While most commercial automated vehicles currently use state machine-based algorithms for trajectory forecasting, recent efforts have focused on end-to-end data-driven systems. Often, the design of these models is limited by the availability of datasets, which are typically restricted to generic scenarios. To address this limitation, we have developed a synthetic dataset for short-term trajectory prediction tasks using the CARLA simulator. This dataset is extensive and incorporates what is considered complex scenarios - pedestrians crossing the road, vehicles overtaking - and comprises 6000 perspective view images with corresponding IMU and odometry information for each frame. Furthermore, an end-to-end short-term trajectory prediction model using convolutional neural networks (CNN) and long short-term memory (LSTM) networks has also been developed. This model can handle corner cases, such as slowing down near zebra crossings and stopping when pedestrians cross the road, without the need for explicit encoding of the surrounding environment. In an effort to accelerate this research and assist others, we are releasing our dataset and model to the research community.


# Perspective View Images from Carla

This repository contains a collection of perspective-view images captured from the Carla simulator. The images are intended for research and development purposes in the field of computer vision, machine learning, and autonomous driving.

## Dataset Description

The dataset comprises a set of perspective-view images captured from different camera angles and positions within the Carla simulator environment. The images are saved in PNG format and have a resolution of 1280x720 pixels. Each image is associated with a timestamp indicating the time of capture.


## Usage

The images in this dataset can be used for various purposes, including:

- Training and evaluating computer vision algorithms
- Developing and testing machine learning models for object detection, semantic segmentation, or other vision tasks
- Conducting research in the field of autonomous driving and perception systems

## Citation👇🏻

If you use this dataset in your research or work, we kindly request that you cite the following paper:

[Insert paper citation here]

## Download Dataset 📈

To access the dataset, please click [here](https://drive.google.com/drive/folders/1JPb64bGV88ymZkJrUBaKQg12tToZVF7T?usp=sharing) to visit the download page.


<!---
<div style="display: flex;">
  <img src="https://github.com/sharmasushil/Navigating-Uncertainty-Trajectory-Prediction/assets/70905483/5b6d04b4-ad09-4927-a783-2f3e70d9e02d" alt="Screenshot 1" width="400">
  <img src="https://github.com/sharmasushil/Navigating-Uncertainty-Trajectory-Prediction/assets/70905483/a64bd0f7-c4e8-4d58-b4d7-43e7a4690b24" alt="Screenshot 2" width="400">
</div>
-->





![Screenshot 2023-05-16 at 14 41 50 (1)](https://github.com/sharmasushil/Navigating-Uncertainty-Trajectory-Prediction/assets/70905483/a64bd0f7-c4e8-4d58-b4d7-43e7a4690b24)


## Contact ✉️

For any questions or inquiries regarding the dataset, please contact [sushil.sharma@ul.ie](sushil.sharma@ul.ie).

