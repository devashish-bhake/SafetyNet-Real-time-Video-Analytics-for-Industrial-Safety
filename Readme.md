
# SafetyNet
<div align="center">
  <p>
      <img width="50%" src="images/logo.png")
>
  </p>
</div>
Industrial Safety is essential for promoting worker safety, preventing accidents, ensuring compliance, and enhancing overall operational efficiency in industrial environments. This project aims to develop a real-time video analytics tool that enhances industrial safety by detecting and preventing potential hazards and unsafe situations in industrial environments.

## Objective

The objective of this project is to leverage Deep Learning techniques to monitor live video feeds and provide real-time hazard detection, prompt alerts, and interventions, enhancing industrial safety and preventing accidents in industrial environments.

## Project Structure & Flow
![project_flow](https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety/assets/73399290/5b316604-3b94-4e1d-88ca-73977cba60c0)


## Technologies & Tools

- Python
- OpenCV
- Tensorflow
- YOLO (You Only Look Once) v8
- Flask (APIs and Back-end)
- React (Web-Application / Front-end
- Firebase - Firestore (NoSQL Database)
- RaspberryPi (Sensor Integration)

## Features

- Real-time video analysis for hazard detection.
- Proactive alert system for immediate intervention.
- User-friendly web interface for monitoring and control.
- Integration with existing industrial video data.
- Dashboard for factory managers to track safety statistics and incidents.

## Getting Started

Follow these steps to get started with the project:

1. Clone this repository to your local machine:

   ```bash
   git clone (https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety)https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety)
   cd SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety
   ```
2.  Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Start the application:

   ```bash
   cd flask_api
   python app.py
     ```
   
5. Run web application:

     ```bash
     cd frontend
     npm start
     ```

## Model statistics
### 1. Class labels:
    [Hardhat, Mask, NO-Hardhat, NO-Mask, NO-Safety Vest, Person, Safety Cone,
    Safety Vest, machinery, vehicle]
The model that was used in order to train this model was the **yolov8l** model that consists of 268 layers and 43,668,288 parameters. The model needs approximately 165 GFLOPS of compute power to run.
The model was trained on a custom dataset with the aforementioned classes and the hardware that was required to train that model was: **2x Nvidia Tesla T4 GPUs with 16gb VRAM each, 30GB of RAM and 4v CPU compute Engine.**

The model was trained for **310 epochs** and took a total amount of time of nearly **36 hrs** to train completely.
### 2. Model Metrics:
#### a. mAP50 (B): 
The mAP50 B is the Mean Absolute Precision where it measures the Average Precision of detections that have at least a 50% overlap with ground truth objects while excluding those overlapping with the background.
![Screenshot from 2023-09-03 15-24-39](https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety/assets/79623853/bb479f2b-5d73-4feb-9c57-0f077a78ac54)
#### b. mAP_0.5: 
The mAP_0.5 is the same as the previous one but in contrast, mAP_0.5 calculates Average Precision based on detections with an Intersection over Union (IoU) of 0.5 or higher with ground truth objects.
![Screenshot from 2023-09-03 15-27-09](https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety/assets/79623853/26fb61a3-26d3-47c3-9ee5-cfaa7558d12f)
#### c. Precision:
Precision in object detection is a metric that assesses the accuracy of a model's detections. It measures the ratio of correctly predicted positive detections to the total number of positive predictions made by the model. In the context of object detection, a "positive detection" refers to a bounding box or region proposed by the model that correctly corresponds to an actual object in the scene.
![Screenshot from 2023-09-03 15-29-52](https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety/assets/79623853/3c860263-adca-45c6-9bee-e8ad0f5ea24f)
#### d. Recall:
Recall, in the context of object detection, is another important metric that evaluates the completeness of a model's detections. It measures the ratio of correctly predicted positive detections to the total number of actual positive objects present in the scene.
![Screenshot from 2023-09-03 15-31-06](https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety/assets/79623853/b2dfbb69-57dd-4e88-8877-86c90c32cb34)
## Usage
- Upload industrial video data for analysis.
- The system will analyze the video in real-time, detecting potential hazards.
- The dashboard provides real-time statistics on safety incidents.
- When a hazard is detected, the system triggers alerts and interventions as needed.

## Outputs
### 1. Safety Gear Recognition: 
![outputgif](https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety/blob/main/images/output.gif?raw=true)

### 2. Emergency Hand Gesture Detection:
![output2](https://github.com/smartinternz02/SBSPS-Challenge-10024-SafeZone-Real-time-Video-Analytics-for-Industrial-Safety/blob/main/images/2cb45385-63c5-4336-8bd8-7157e799c460.jpeg?raw=true)
