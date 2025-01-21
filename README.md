# Autonomous Vehicle Object Detection Using YOLOv8 and CARLA 

## Overview
This project demonstrates the integration of real-time object detection in an autonomous vehicle using the CARLA simulator and the YOLOv8 model. The system identifies pedestrians and traffic lights in a dynamic urban environment and modifies vehicle behavior accordingly.

---

## Features
- **CARLA Integration**: Simulates urban driving scenarios with realistic environments.
- **YOLOv8 Object Detection**: Detects pedestrians, traffic lights, and other objects. To improve detection accuracy, only objects with a confidence level above 0.6 (on a scale of 0 to 1) are processed. This filtering ensures that the system reacts only to reliable detections.
- **Real-Time Action**: Slows down the vehicle by 50% for 5 seconds when a pedestrian is detected, similar to how real-world vehicles respond to nearby pedestrians.
- **RGB Camera Processing**: Captures and processes live feed from an onboard camera for continuous object detection.

---

### Components
1. **CARLA Simulator**:
   - Simulates a city environment (Town02) with pedestrians, vehicles, and traffic lights.
   - Provides sensor data (camera feed) for processing.

2. **YOLOv8 Integration**:
   - Processes images from the RGB camera.
   - Identifies objects such as pedestrians and traffic lights with confidence thresholds.

3. **Autonomous Vehicle Behavior**:
   - The vehicle operates on autopilot.
   - When a pedestrian is detected, the Traffic Manager adjusts the speed.

---

### Workflow
1. The CARLA simulator initializes the urban environment and spawns vehicles and pedestrians.
2. The onboard RGB camera captures live video.
3. Images are processed with YOLOv8 to detect objects.
4. If a pedestrian is detected:
   - The Traffic Manager reduces the vehicle's speed by 50% for 5 seconds.
5. The system logs detection details and overlays bounding boxes on detected objects.

---

### Video Demonstration

[![Watch the video demonstration](https://drive.google.com/thumbnail?id=1YoiyYKKcEb6YuYje_Ls3Pfg4JML29rqE)](https://drive.google.com/file/d/1YoiyYKKcEb6YuYje_Ls3Pfg4JML29rqE/view?usp=drive_link)


---

## Screenshots

### Detection Visualization

![Picture2](https://github.com/user-attachments/assets/d692c9be-764e-4456-8234-7146e282979c)

![Picture1](https://github.com/user-attachments/assets/799b4fba-6d57-4366-980c-4ea10fc45941)


---
