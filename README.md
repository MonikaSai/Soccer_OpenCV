# Soccer_OpenCV
Player_detection, Ball_detection, Machine Learning, Annotations, Python

# Dependencies
Python3, tensorflow, numpy, opencv3, pillow, sklearn

## Getting Started 

1. https://github. com/thtrieu/darkflow - darkflow is used for ball_tracking by own annotated dataset.
![ball_tracking](https://user-images.githubusercontent.com/54144435/92119083-40e5f380-edef-11ea-8d26-b413eb2b151c.gif)

2. https://github.com/Qidian213/deep_sort_yolov3  - deep_sort_yolov3 is used for the player_detection
![player_detection](https://user-images.githubusercontent.com/54144435/92119204-6672fd00-edef-11ea-9f19-2bfa918b5b34.gif)

![player_detection_dis and speed](https://user-images.githubusercontent.com/54144435/92119346-94f0d800-edef-11ea-9a3e-d4a42e3bfcee.gif)

3. Filed Detection - python

![field detection](https://user-images.githubusercontent.com/54144435/92119262-77bc0980-edef-11ea-8017-96bce109042f.gif)

### Player Detection and Ball Detection in Soccer Videos

There are multiple ways to detect players in any sports videos.Here I have used simple image processing techniques to detect players by only using opencv.

If the Dataset is clear there are the possibilities of implementing few more features.

It detects first the green ground and make everything other then green color into black.After converting into greyscale I have found contours on the ground.By using some parameters we will detect players.

Here I have used the video of France VS Belgium match.So for further detection, I have used the color of their jersy to segment them.For france We will detect the blue jersy and then for belgium we will detect the red jersy. 

Algorithm:
First we will read the video.
Detect the Green ground.
Use morphological operation for better detection.
Find contours.
Detect players.
Segment them by France or Belgium.
Detect the soccer ball.

You can see the code in player_detection.py

