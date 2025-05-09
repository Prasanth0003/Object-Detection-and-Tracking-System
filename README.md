# Object Detection and Tracking System

A Python-based object detection and tracking system that uses YOLOv8 for real-time object detection in images, videos, and webcam streams. The application features a user-friendly GUI interface and includes text-to-speech functionality for announcing detected objects.

## Features

- Real-time object detection using YOLOv8
- Support for multiple input sources:
  - Image upload
  - Video file upload
  - Live webcam feed
- Interactive GUI interface
- Text-to-speech announcements of detected objects
- Real-time bounding box visualization
- Object counting and statistics

## Requirements

- Python 3.x
- Required packages (install using `pip install -r object_detection_v5_req.txt`):
  - ultralytics
  - opencv-python
  - numpy
  - pillow
  - pyttsx3
  - tkinter

## Installation

1. Clone this repository or download the source code
2. Install the required dependencies:
   ```bash
   pip install -r object_detection_v5_req.txt
   ```
3. Download the YOLOv8 model file (`yolo11s.pt`) and place it in the project directory

## Usage

1. Run the main application:
   ```bash
   python Main.py
   ```

2. The application provides four main options:
   - **Upload Image**: Select and analyze an image file
   - **Upload Video**: Select and analyze a video file
   - **Start Webcam**: Begin real-time detection using your webcam
   - **Exit**: Close the application

3. For video and webcam modes:
   - Press 'q' to stop the detection and return to the main interface
   - The application will display detected objects in real-time with bounding boxes
   - Text-to-speech will announce detected objects

## Project Structure

- `Main.py`: Main application file containing the GUI and detection logic
- `object_detection_v5_req.txt`: List of required Python packages
- `yolo11s.pt`: YOLOv8 model file (not included, needs to be downloaded separately)

## Features in Detail

### Image Detection
- Upload and analyze single images
- Display bounding boxes around detected objects
- Show object counts and labels
- Text-to-speech announcement of detected objects

### Video Detection
- Process video files frame by frame
- Real-time object detection and tracking
- Display results in the GUI
- Voice announcements of detected objects

### Webcam Detection
- Real-time object detection using webcam feed
- Live visualization of detected objects
- Continuous voice feedback
- Press 'q' to stop detection

## Notes

- The application requires a working webcam for the webcam detection feature
- Text-to-speech functionality requires system audio output
- The YOLOv8 model supports detection of 80 different object classes

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to submit issues and enhancement requests! 
