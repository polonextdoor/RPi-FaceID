# RPi-FaceID: Raspberry Pi 5 Facial Recognition Attendance System

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/your-username/your-repo-name/graphs/commit-activity)
[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-%3E%3D4.x-brightgreen.svg)](https://opencv.org/)
[![Picamera2](https://img.shields.io/badge/Picamera2-Latest-blueviolet.svg)](https://libcamera.org/)

**Track attendance using facial recognition on Raspberry Pi 5**

This project is a face recognition based attendance system built with Python and OpenCV. Leveraging the power of the Raspberry Pi 5 and the **new Picamera2 library**, it captures images of individuals and compares them against a database of known faces to automatically record attendance.

## Key Features

* **Facial Recognition:** Accurately identifies individuals based on their facial features.
* **Attendance Tracking:** Automatically marks attendance records upon successful recognition.
* **Raspberry Pi Powered:** Designed for efficient and low-cost deployment on Raspberry Pi devices.
* **Picamera2 Integration:** Utilizes the latest Picamera2 library for enhanced camera control and performance.
* **OpenCV for Image Processing:** Employs the robust OpenCV library for image capture, preprocessing, and facial recognition algorithms.
* **Easy to Use:** Simple setup and configuration for quick deployment.

## Getting Started

### Prerequisites

* Raspberry Pi 5
* Raspberry Pi Camera Module (v2 or **Picamera2 compatible**)
* Python 3.11
* OpenCV (`pip install opencv-python`)
* **Picamera2 Library** (`pip install picamera2`)
* All other necessary libraries (install via `pip install -r requirements.txt` or manually using pip)

### Installation
Clone the repository to your local machine. git clone https://github.com/polonextdoor/RPi-FaceID
* Install the required packages using pip install -r requirements.txt.
* Download the dlib models from [dlib face recognition resnet model](https://drive.google.com/drive/folders/1M4f7WV2wZuJmlAKkh4IWdOMJJ3K5Cdb3?usp=sharing) and place the data folder inside the repo
* **Ensure Picamera2 is properly configured on your Raspberry Pi.** Refer to the official Picamera2 documentation for installation and setup instructions: [https://libcamera.org/](https://libcamera.org/)

### Usage

* Collect the Faces Dataset by running  python get_faces_from_camera_tkinter.py .
* Convert the dataset into python features_extraction_to_csv.py.
* To take the attendance run python attendance_taker.py .
* Check the Database by python app.py.

### Thanks to Arijit1080 for his repo providing a foundation for this project
https://github.com/Arijit1080/Face-Recognition-Based-Attendance-System
