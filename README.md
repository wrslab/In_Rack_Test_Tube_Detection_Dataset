# Dataset for the paper "Automatically Prepare Training Data for YOLO Using Robotic In-Hand Observation and Synthesis" 

This repository contains the datasets, models, test results and for the paper "Automatically Prepare Training Data for YOLO Using Robotic In-Hand Observation and Synthesis". We proposed combining robotic in-hand observation and data synthesis to enlarge the limited data set. We first used a robot with a depth sensor to collect images of objects held in the robot's hands and segment the object pictures. Then, we used a copy-paste method to synthesize the segmented objects with rack backgrounds. The collected images and the synthetic ones are combined to train a deep detection neural network. We conducted experiments to compare YOLOv5x detectors trained with images collected using the proposed method and several other methods. The results showed that combined observation and synthetic images led to comparable performance to manual data preparation. They provided a good guide on optimizing data configurations and parameter settings for training detectors. The proposed method required only a single process and was a low-cost way to produce the combined data.

## Changelog
[Oct 2022] Initial release of TubeDet
 
## Datasets and Weights
The datasets used in the Table II of the paper.

| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| | 
|RO1600| | |
|SR1600| | |
|SB1600| | |
|RO1600+SR800| | |
|RO1600+SB800| | |
|SR800+SB800| | | 

---

The datasets used in the Table III of the paper.
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|RO800+SR200| | 
|RO800+SR400| | |
|RO800+SR800| | |
|RO800+SR1600| | |
|RO200+SR800| | |
|RO400+SR800| | |
|RO1600+SR800| | |

---

The datasets used in the Table IV of the paper.
| Params,(T,t)| Dataset links | Weight links |
| :----: | :----: | :----: |
|(10,.10)| | |
|(20,.10)| | |
|(30,.10)| | |
|(40,.10)| | |
|(30,.20)| | |
|(30,.40)| | |
|(30,.60)| | |
|(30,.80)| | |

---

The datasets used in the Table V of the paper.
| #Caps| Dataset links | Weight links |
| :----: | :----: | :----: |
|200| | |
|400| | |
|800| | |
|1600| | |
 
---

The datasets used in the Table VI of the paper.
| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|SB200+SR800| | 
|SB400+SR800| | |
|SB600+SR800| | |
|SB800+SR800| | | 
|SB1600+SR800| | | 
|SB800+SR200| | 
|SB800+SR400| | |
|SB800+SR600| | |
|SB800+SR800| | | 
|SB800+SR1600| | | 

 
