
<p align="center">
    <h3 align="center"><a href="https://arxiv.org/pdf/2307.05288.pdf">📑 Article</a>  | <a href="https://drive.google.com/drive/folders/1JPb64bGV88ymZkJrUBaKQg12tToZVF7T?usp=sharing">📂 Dataset</a> | <a href="https://youtu.be/DZDqGbkInko">🎬 Video</a> </h3>
</p>

# Navigating Uncertainty: The Role of Short-Term Trajectory Prediction in Autonomous Vehicle Safety 🚘
Abstract: Autonomous vehicles require accurate and reliable short-term trajectory predictions for safe and efficient driving. While most commercial automated vehicles currently use state machine-based algorithms for trajectory forecasting, recent efforts have focused on end-to-end data-driven systems. Often, the design of these models is limited by the availability of datasets, which are typically restricted to generic scenarios. To address this limitation, we have developed a synthetic dataset for short-term trajectory prediction tasks using the CARLA simulator. This dataset is extensive and incorporates what is considered complex scenarios - pedestrians crossing the road, vehicles overtaking - and comprises 6000 perspective view images with corresponding IMU and odometry information for each frame. Furthermore, an end-to-end short-term trajectory prediction model using convolutional neural networks (CNN) and long short-term memory (LSTM) networks has also been developed. This model can handle corner cases, such as slowing down near zebra crossings and stopping when pedestrians cross the road, without the need for explicit encoding of the surrounding environment. In an effort to accelerate this research and assist others, we are releasing our dataset and model to the research community.



# Perspective View Images from Carla 📌

This repository contains a collection of perspective-view images captured from the Carla simulator. The images are intended for research and development purposes in the fields of computer vision, machine learning, and autonomous driving.

# Architecture Topology ⛓️

The network developed in this work is designed to predict the future trajectories of a vehicle based on a sequence of perspective-view images. It comprises two primary components: a Convolutional Neural Network (CNN) and a Long-Short Term Memory Network (LSTM

The following diagram illustrates a suggested topology for a CNN architecture designed to estimate trajectories from image sequences. It highlights the progression of information flow across convolutional and fully connected layers.


<img src="https://github.com/sharmasushil/Navigating-Uncertainty-Trajectory-Prediction/assets/70905483/45e80d08-a5a7-4f44-86b3-3ac89846fb31" width = "850">



## Dataset Description: 💻

The dataset comprises a set of perspective-view images captured from different camera angles and positions within the Carla simulator environment. The images are saved in PNG format and have a resolution of 800 x 600 pixels. Each image is associated with a timestamp indicating the time of capture.

## Ablation study 
An ablation study on the number of LSTM cells ($\alpha$=1, $\beta$=2, $\gamma$=3, $\delta$=4) is conducted on our CNN-LSTM model. This comparison was performed using the CARLA dataset for the two specified levels, Level 1 and Level 2 respectively. For this analysis, three evaluation metrics - RMSE, MAPE, and AED. A summary of the results is shown in Table \ref{table:3}.

| CARLA: Dataset | Model | ARMSE ↓ | AMAPE ↓ | AED ↓ |
|---|---|---|---|---|
| Dataset: Level 1 | CNN-LSTM ($\alpha$)<br>   CNN-LSTM ($\beta$)<br>  CNN-LSTM ($\gamma$)<br> **CNN-LSTM ($\delta$)**   | 0.0046<br>  0.0034<br>  0.0028<br> **0.0024** | 0.0056<br>  0.0043<br>  0.0038<br> **0.0033** | 0.0050<br>  0.0039<br>  0.0032<br>  **0.0028** |
| Dataset: Level 2 | CNN-LSTM ($\alpha$)<br>  CNN-LSTM ($\beta$)<br>   CNN-LSTM ($\gamma$)<br>  **CNN-LSTM ($\delta$)**| 0.0126<br>  0.0097<br>  0.0082<br> **0.0065**  | 0.0172<br>  0.0133<br>  0.0119<br> **0.0107** | 0.0154<br>  0.0127<br>  0.0107<br> **0.0079** |




## Usage ⚙️

The images in this dataset can be used for various purposes, including:

- Training and evaluating computer vision algorithms
- Developing and testing machine learning models for trajectory prediction, object detection, semantic segmentation, or other vision tasks
- Conducting research in the field of autonomous driving and perception systems

## Citation👇🏻

If you use this dataset in your research or work, we kindly request that you cite the following paper:

```BibTeX
@inproceedings{sharma2023navigating,
      title={Navigating Uncertainty: The Role of Short-Term Trajectory Prediction in Autonomous Vehicle Safety}, 
      author={Sushil Sharma and Ganesh Sistu and Lucie Yahiaoui and Arindam Das and Mark Halton and Ciarán Eising},
      year={2023},
      booktitle={Proceedings of the Irish Machine Vision and Image Processing Conference}
}
```





## Download Dataset 📂

To access the dataset, please click [Dataset Download (< 1 GB)](https://drive.google.com/drive/folders/1JPb64bGV88ymZkJrUBaKQg12tToZVF7T?usp=sharing)  to visit the download page.

#### Data statistics for each class of our newly created dataset

<img src="https://github.com/sharmasushil/Navigating-Uncertainty-Trajectory-Prediction/assets/70905483/a6c4bcfa-67d0-4420-8739-b25328dd92a0" width = "850">





## CARLA Results Visualization 📈
We showcase the resilience of our model in dealing with challenging scenarios, including pedestrian crossings, without relying on the explicit encoding of contextual information. The figure below illustrates a comparison between Ground Truth (shown in blue) and Predicted Bounding Boxes (highlighted in red) for trajectory prediction.

<img src="https://github.com/sharmasushil/Navigating-Uncertainty-Trajectory-Prediction/assets/70905483/28714df0-6f9d-4048-b51b-bbd43c4deb62" width = "850">





## Contact ✉️




For any questions or inquiries regarding the dataset, please contact sushil.sharma@ul.ie

