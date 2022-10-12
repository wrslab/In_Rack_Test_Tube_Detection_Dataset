# Dataset for the paper "Automatically Prepare Training Data for YOLO Using Robotic In-Hand Observation and Synthesis" 

This repository contains the datasets, models, test results and for the paper "Automatically Prepare Training Data for YOLO Using Robotic In-Hand Observation and Synthesis". We proposed combining robotic in-hand observation and data synthesis to enlarge the limited data set. We first used a robot with a depth sensor to collect images of objects held in the robot's hands and segment the object pictures. Then, we used a copy-paste method to synthesize the segmented objects with rack backgrounds. The collected images and the synthetic ones are combined to train a deep detection neural network. We conducted experiments to compare YOLOv5x detectors trained with images collected using the proposed method and several other methods. The results showed that combined observation and synthetic images led to comparable performance to manual data preparation. They provided a good guide on optimizing data configurations and parameter settings for training detectors. The proposed method required only a single process and was a low-cost way to produce the combined data.

## Changelog
[Oct 2022] Initial release of TubeDet
 
## Setup
Check [YOLOv5](https://github.com/ultralytics/yolov5) repo for details

1. Value the weights by 
```
python .\val.py --weight [weight_option] --img 1376 --data [val_dataset_yaml]
``` 
Change the `[weight_option]` to the path of the weight and change the `[val_dataset_yaml]` to the yaml file of the testing data

2. Value 

## Datasets and Weights
The datasets and weights used in the Table II of the paper.

| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|CL200| [Google Drive](https://drive.google.com/file/d/1o_GysrCxgZ4evxOy9U1NoqxmBXhzqCAx/view?usp=sharing) |[Google Drive](https://drive.google.com/file/d/1Jdg4l6_7SFoGY1qSYZxhF_w7LzRIPYUl/view?usp=sharing) | 
|RO1600| [Google Drive](https://drive.google.com/file/d/1bclJbhRXgGiRFjk2ZY1Ec_o33hQ__15v/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1AG2f6lc4VtoxhoXVwDIqCRV-rSL8N4jA/view?usp=sharing) |
|SR1600| [Google Drive](https://drive.google.com/file/d/1daTh6-bJmTEB591Habbsmqf2PSqsj6AA/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1HHdR2EPa3tlNSJkYzUfaZNNzlgxKqRw5/view?usp=sharing) |
|SB1600|[Google Drive](https://drive.google.com/file/d/1KC80mR-iO4csqmUPfJtQ00MGWK4Jkc9q/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1pajWljRSzOhiuK7AvrdopOI2BO10spk7/view?usp=sharing)|
|RO1600+SR800| [Google Drive](https://drive.google.com/file/d/1WAXnm7OYBK1xFyrRDs8_icCvfAPB7cGQ/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1KmowYCw21mH6TRPa2XQ4xH-_49FAYAmq/view?usp=sharing) |
|RO1600+SB800| [Google Drive](https://drive.google.com/file/d/1o8B8hQQQa5khTG_OIOa2XwTCoRBmp_IU/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1Y9wuuzRPDFNiv4ODmnJa7cKlxFjtpe7W/view?usp=sharing)|
|RO1600+SR400+SB400| [Google Drive](https://drive.google.com/file/d/1bxhNHoKG7lIWf3eFaQavOztty-CgIAg6/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1VxFnEsCQuVrzLfJOa3vzQNFr2TB87TuD/view?usp=sharing) |
|SR800+SB800| [Google Drive](https://drive.google.com/file/d/1b0EkzFMlH7smpIH_jaBBXfiAuspLCQxB/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_Tt9h6ojqrt9UtJ4K5IKLTcr4IuJq4DI/view?usp=sharing)| 

---

The datasets and weights used in the Table III of the paper.

| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|RO800+SR200| | 
|RO800+SR400| | |
|RO800+SR800| | |
|RO800+SR1600| | |
|RO200+SR800| | |
|RO400+SR800| | |
|RO1600+SR800| [Google Drive](https://drive.google.com/file/d/1WAXnm7OYBK1xFyrRDs8_icCvfAPB7cGQ/view?usp=sharing)|[Google Drive](https://drive.google.com/file/d/1KmowYCw21mH6TRPa2XQ4xH-_49FAYAmq/view?usp=sharing) |

---

The datasets and weights used in the Table IV of the paper.

| Params,(T,t)| Dataset links | Weight links |
| :----: | :----: | :----: |
|(10,.10)|  | |
|(20,.10)| [Google Drive](https://drive.google.com/file/d/149lGnaz2ePSJh2kbldaXQMGFyCv_2er0/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1IAp68JWeKUjYOQCTHo348uWO5AlWKxEv/view?usp=sharing)|
|(30,.10)| [Google Drive](https://drive.google.com/file/d/1K2pnUW3obE8VaVGGYukWZmQiQZb-q-Le/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1M7U7ry32nplNEoSmnSevDv_OF_nr_X2k/view?usp=sharing)|
|(40,.10)|  | |
|(30,.20)| | |
|(30,.40)| [Google Drive](https://drive.google.com/file/d/1UWxS2PmXlTKw6KMpxM7in9263M49dGJc/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1x8NJerGezxP__nInmlUjy7HLRT0D-C1M/view?usp=sharing)|
|(30,.60)| [Google Drive](https://drive.google.com/file/d/16-lLsoQaxdndZRKcX4KFo9CFm69OCvQ3/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1aaPNMDYSYnvjsDWC3iB_uLZbZxtNvDdo/view?usp=sharing)|
|(30,.80)| [Google Drive](https://drive.google.com/file/d/106cPWysI56nv_C_3xDABxatPIGjv7AEW/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1y44XvwGUkkSPir61OA8IRbx33hMoIvQE/view?usp=sharing)|

---

The datasets and weights used in the Table V of the paper.

| #Caps| Dataset links | Weight links |
| :----: | :----: | :----: |
|400| [Google Drive](https://drive.google.com/file/d/14qyNUPHDe6f7bT1EX5YOrp-vF4F6gMUr/view?usp=sharing)| |
|800| [Google Drive](https://drive.google.com/file/d/1HxOuIEaejJcEsfHXRZBBzEWlg7NeDQCI/view?usp=sharing)| |
|1600| [Google Drive](https://drive.google.com/file/d/15NlkB5oG6gJUU6xSLCvDj5DepJqd_kMj/view?usp=sharing)| |
|3200| [Google Drive](https://drive.google.com/file/d/1b0EkzFMlH7smpIH_jaBBXfiAuspLCQxB/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_Tt9h6ojqrt9UtJ4K5IKLTcr4IuJq4DI/view?usp=sharing)| 
 
---

The datasets and weights used in the Table VI of the paper.

| Dataset Names| Dataset links | Weight links |
| :----: | :----: | :----: |
|SB200+SR800| [Google Drive](https://drive.google.com/file/d/1E5BUioUtqmev5qrIPXpp40BgE_lPOlTA/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1og021q1ajWo6cFb4-0VcArNgOmlxaXaV/view?usp=sharing)|
|SB400+SR800| [Google Drive](https://drive.google.com/file/d/13seAmvoGqMM-_KNpYFtNQtbrDctcXeha/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1PwLdCS5Vw0rHBUb9ozFzolyObuh0VDea/view?usp=sharing)|
|SB600+SR800| [Google Drive](https://drive.google.com/file/d/1vg3JWr4QzDVV8waiAllT8-G4prv7tD3L/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1Zh6zCpn9ZZiuOhfZtDnHvp4oVNRVkT0r/view?usp=sharing) |
|SB800+SR800| [Google Drive](https://drive.google.com/file/d/1b0EkzFMlH7smpIH_jaBBXfiAuspLCQxB/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_Tt9h6ojqrt9UtJ4K5IKLTcr4IuJq4DI/view?usp=sharing)| 
|SB1600+SR800| [Google Drive](https://drive.google.com/file/d/1BeCMifrb4nj5WZO-kF-qFWGK_0dGTUry/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1zhFkIADevgVDdvcVpJ6V_dJPjxUF3Bw-/view?usp=sharing)| 
|SB800+SR200| [Google Drive](https://drive.google.com/file/d/1OQyIEN3ylzVpGz--dFjv725McUl4i9Yt/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1vg3JWr4QzDVV8waiAllT8-G4prv7tD3L/view?usp=sharing)| 
|SB800+SR400| [Google Drive](https://drive.google.com/file/d/11zcDCVs-PgJ5P7fp11u5JdsSblo13R56/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1wQsvuyjEhH6bVr-mu0hRpNAQL6p7-IwC/view?usp=sharing)|
|SB800+SR600| [Google Drive](https://drive.google.com/file/d/1C1_7Kq2An1MlO20-0HSOYxwdm_ueYaYV/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1gktpxa6qpEniMsj8RardqlTBL1bqmucS/view?usp=sharing)|
|SB800+SR800| [Google Drive](https://drive.google.com/file/d/1b0EkzFMlH7smpIH_jaBBXfiAuspLCQxB/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1_Tt9h6ojqrt9UtJ4K5IKLTcr4IuJq4DI/view?usp=sharing)| 
|SB800+SR1600| [Google Drive](https://drive.google.com/file/d/1FdkHEZSGX9h7dibXWH4iNKudmWphyGaL/view?usp=sharing)| [Google Drive](https://drive.google.com/file/d/1cv1ZYWzfvknaBIKvxe_N31tMggcQ1LdV/view?usp=sharing)| 

 
