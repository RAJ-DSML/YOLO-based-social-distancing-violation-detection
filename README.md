# YOLO-based-social-distancing-violation-detection

<!-- Objective -->
### Objective

Covid 19 can be prevented if few norms are followed properly. Social Distancing is one of the important norms to stops spreading COVID-19. Advance Computer Vision technique can be implemented to identified if few persons are maintaining social distance or not. This can be used to spread awareness.

<!-- Problem Statement -->
### Problem Statement
* MAIN GOAL: To identify whether the people are in adequate distance or not. 
* RED: High Risk; GREEN: Safe
* DISTANCE METRIC: Euclidean Distance.
* Used Deep Learning/ Computer Vision technique.

<!-- Prerequisites -->
### Prerequisites

You need to install following python packages along with Jupyter Notebook.

* tensorflow
  ```sh
  pip install tensorflow
  ```
* opencv
  ```sh
  pip install opencv-python
  ```
* scipy
  ```sh
  pip install scipy
  ```
* imutils
  ```sh
  pip install imutils
  ```
  
### Methods
* The backbone of our pre-trained model is YOLO v3.
* Here we use supporting weights for the architecture trained with the COCO data set.
* Measured the distance between two persons using “Euclidean/L2 Norms”.

### Dataset
* As the objective of the project is to work with CCTV footages, we considered a real-world video as our dataset.
* The test dataset is a recorded video of 3351 number of frames (720P - 30 FPS).
* Configuration : Android Phone with 48 Mega-Pixel Image Sensor
* Location : Bandel, West Bangal.

### Initial Result
<p align="center">
  <a href="https://github.com/RAJ-DSML/YOLO-based-social-distancing-violation-detection/blob/main/img/initial_result.JPG">
    <img src="https://github.com/RAJ-DSML/YOLO-based-social-distancing-violation-detection/blob/main/img/initial_result.JPG" alt="Logo" width="800" height="500">
  </a>
  
 * At the initial stage the model is detecting almost all the object present in the video as well as in the coco data set.
 * We need to filter out only human beings.
  
 ### Final Result
  <p align="center">
  <a href="https://github.com/RAJ-DSML/YOLO-based-social-distancing-violation-detection/blob/main/img/final_result.JPG">
    <img src="https://github.com/RAJ-DSML/YOLO-based-social-distancing-violation-detection/blob/main/img/final_result.JPG" alt="Logo" width="800" height="500">
  </a>
   
 The model is detecting only the human beings and calculating the distance between the nearest bounding box. This is how it is taking a decision between high risk and safe distances.
   
### Conclusion
    
* The Final model is taking the decision based upon the pixel distance which can be modified based upon the recommendations by the experts.
* As the model is robust it can be used for any type of videos recorded from various devices (e.g.: Mobile Phones, CCTV footages, Cameras, Drones etc.) 

Output Video Link : https://www.facebook.com/100009251473110/videos/pcb.2902819053369782/2902807873370900
