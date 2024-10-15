# **Pulse Rate Detection using OpenCV and Dlib**

This project demonstrates how to determine the pulse rate of a person by analyzing forehead pulse points captured from a video. The pulses, which are not visible to the naked eye, are detected using **computer vision (CV)** techniques. The **Dlib** library is used to capture facial landmarks, and **OpenCV** processes the frames to extract forehead pulses. The result is visualized with a graph representing the subject's pulse over time.

---

## **Table of Contents**
- [Overview](#overview)  
- [Features](#features)  
- [Installation](#installation) 
- [Technologies Used](#technologies-used)  
 

---

## **Overview**
The pulse rate of a person is detected by analyzing minute changes in forehead color patterns, which correspond to heartbeats. A video of the person, captured while they remain stable, is processed to extract these subtle pulses. **Dlib's facial landmark detector** is used to identify facial regions, particularly the forehead. **OpenCV** processes frames, and sampling techniques are applied to generate a **pulse rate graph**.

---

## **Features**
- Detects pulse rate from a video of a person’s face.
- Uses **Dlib** for facial landmark detection to capture the forehead region.
- Processes each frame using **OpenCV** to analyze color changes over time.
- Generates a **graph** representing the pulse rate.
- Can be used for contactless heart rate monitoring.

---

## **Installation**

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/pulse-rate-detection.git
   cd pulse-rate-detection
2. Create a Virtual Environment:
python -m venv env
source env/bin/activate    # On Linux/macOS
env\Scripts\activate       # On Windows

4. Install Dlib (if not installed):
On Windows, use pre-built wheels:
- pip install dlib
On Linux/macOS, ensure CMake is installed
- pip install cmake
- pip install dlib

##**Technologies Used**
Python: Core language for development.
OpenCV: For video frame processing.
Dlib: To detect facial landmarks.
Matplotlib: To plot the pulse rate graph.
NumPy: For data handling and frame analysis.
