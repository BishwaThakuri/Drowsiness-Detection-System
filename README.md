# Drowsiness Detection System

This project is a real-time drowsiness detection system that utilizes computer vision and machine learning techniques to detect if a person is falling asleep based on eye aspect ratio (EAR). It uses OpenCV for video capture and facial landmark detection, dlib for face detection, and pyttsx3 for text-to-speech alerts.

## Features
- Real-time detection of drowsiness based on eye closure.
- Visual alerts on the display.
- Audio alerts using a text-to-speech engine.

## Requirements
- Python 3.x
- OpenCV
- dlib
- pyttsx3
- scipy

## Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/BishwaThakuri/Drowsiness-Detection.git
    cd Drowsiness-Detection
    ```

2. Install the required dependencies:
    ```bash
    pip install opencv-python dlib pyttsx3 scipy
    ```

3. Download the facial landmark predictor:
    - Download the `shape_predictor_68_face_landmarks.dat` file from [dlib's model repository](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2).
    - Extract the `.dat` file and place it in the project directory.

## Running the Application
1. Run the Python script.

2. The application will start the camera and monitor for signs of drowsiness. To stop the application, press `q`.

## How It Works
- The system captures video frames and detects faces using dlib’s frontal face detector.
- It then locates facial landmarks and calculates the Eye Aspect Ratio (EAR) to determine eye closure.
- If the EAR falls below a certain threshold, the system detects drowsiness and issues both visual and audio alerts.

## Key Components
- **OpenCV**: For capturing video frames and processing images.
- **dlib**: For facial detection and landmark identification.
- **pyttsx3**: For providing audio alerts using text-to-speech.
- **scipy**: For calculating distances between facial landmarks.

## Usage
This system can be used in vehicles to alert drivers when they show signs of drowsiness, potentially preventing accidents caused by falling asleep at the wheel.

## Acknowledgements
- [OpenCV](https://opencv.org/)
- [dlib](http://dlib.net/)
- [pyttsx3](https://pypi.org/project/pyttsx3/)
- [scipy](https://www.scipy.org/)

