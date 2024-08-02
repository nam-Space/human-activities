![image](https://github.com/user-attachments/assets/696d121e-2dfb-4a2e-8ee8-3812d8316d22)# Human Behavior Recognition using OpenCV

This project focuses on recognizing and classifying human behaviors using OpenCV, a powerful open-source computer vision and machine learning software library. The application can detect and interpret various human actions from video feeds or recorded videos.

![image](https://github.com/user-attachments/assets/72532ca8-83c7-4146-b999-51e218da8983)

## Table of Contents

-   [Introduction](#introduction)
-   [Features](#features)
-   [Technologies Used](#technologies-used)
-   [Installation](#installation)
-   [Usage](#usage)

## Introduction

Human behavior recognition is an essential task in computer vision with applications in security, healthcare, human-computer interaction, and more. This project uses OpenCV to detect human behaviors such as walking, running, jumping, and other activities from video feeds.

![image](https://github.com/user-attachments/assets/be457b43-a66b-4a95-86c0-0f2fff3c82a4)

## Features

-   Real-time human behavior recognition from webcam or video files.
-   Support for multiple behaviors like walking, running, jumping, etc.
-   Visual feedback with bounding boxes and labels around detected humans.
-   Easy to extend with new behaviors.

## Technologies Used

-   **Programming Language**: Python
-   **Computer Vision Library**: OpenCV, mediapipe, pandas, scikit-learn
-   **Machine Learning**: TensorFlow/Keras

## Installation

1. Install VS Code or Pycharm

2. Clone the repository:

    ```bash
    git clone https://github.com/nam-Space/human-activities.git
    cd human-activities

    ```

3. Install library:

    ```bash
    pip install opencv-python
    pip install mediapipe
    pip install numpy
    pip install threading
    pip install tensorflow
    pip install pandas
    pip install keras
    pip install scikit-learn
    ```

## Usage

1. Go to `constants.py` and change 2 actions you want to have (example: I want action 1 to `waving` and action 2 to `running`)

    ![image](https://github.com/user-attachments/assets/b37ce38d-0fbc-4292-ad0a-adc20b11e618)

2. Go to `make_data.py` to write data to `{action1}.txt` for the first action by running command `py make_data.py` and doing your action in front of your camera (example: I want to write data of the action `waving` first, then we will have `WAVING.txt`)

    ![image](https://github.com/user-attachments/assets/5b80cd8a-c4b7-4312-938d-b8922aec4129)

    ![image](https://github.com/user-attachments/assets/7b9f9191-1a62-498b-a94f-9b55ad18fd9e)

3. Similarly with second action, we write data to `{action2}.txt` for the second action by changing key of constants `action1` to `action2`, then running command `py make_data.py`, after that you have to do your action in front of your camera (example: I want to write data of the action `running`, then we will have `RUNNING.txt`)

    ![image](https://github.com/user-attachments/assets/5f254230-cfb1-4547-8eac-6324fb72dd66)

    ![image](https://github.com/user-attachments/assets/22dbc0f1-2842-483a-9cc8-e1b28dbe788c)

4. We go to `train_lstm.py` to train all models of `{action1}.txt` and `{action2}.txt` by running command `py train_lstm.py`, then we will have `model.h5` file (example: I want to train all models of `WAVING.txt` and `RUNNING.txt`)

    ![image](https://github.com/user-attachments/assets/8fb875a8-7fd8-4b43-8fb8-286b3a0ecdab)

    ![image](https://github.com/user-attachments/assets/055b2d86-4006-4b90-a8ba-3d86342bac60)

5. We go to `inference_lstm.py` by running command `py inference_lstm.py` then do the action you want, you will see the result
   ![image](https://github.com/user-attachments/assets/f03c0906-956d-4cb0-b6f2-fa50a6456910)

    ![image](https://github.com/user-attachments/assets/956c05ba-3cce-4ecd-b959-b4237f718f93)

    ![image](https://github.com/user-attachments/assets/03d10131-c519-406d-8646-b3384e744bcc)
