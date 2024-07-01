# OBJECT_DETECTION_USING_YOLO

## Project Title
OBJECT_DETECTION_USING_YOLO

## Project Description
This project demonstrates object detection using the YOLOv8n model in a Streamlit application. Users can upload a video file, and the application will perform real-time object detection on the video frames, displaying the detected objects with bounding boxes and class labels. The project leverages the COCO-pretrained YOLOv8n model for accurate and efficient object detection.

## Table of Contents
1. Project Goals
2. Installation
3. Usage Instructions
4. Code Explanation
5. Credits
6. Additional Notes

## Project Goals
- To provide a user-friendly interface for object detection using YOLOv8n.
- To enable users to upload video files and perform real-time object detection.
- To display the detected objects with bounding boxes and class labels on the video frames.

## Installation
1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/OBJECT_DETECTION_USING_YOLO.git
   cd OBJECT_DETECTION_USING_YOLO
   ```

2. **Install required libraries:**
   Make sure you have Python installed. Then, install the necessary libraries using pip:
   ```sh
   pip install streamlit opencv-python-headless numpy ultralytics
   ```

3. **Download the YOLOv8n weights:**
   Place the YOLOv8n weights file (`yolov8n.pt`) in the `weights` directory.

4. **Ensure you have the COCO class names file:**
   Make sure the `coco.txt` file containing the class names is in the correct directory.

## Usage Instructions
1. **Run the Streamlit application:**
   ```sh
   streamlit run app.py
   ```

2. **Upload a video file:**
   - Open the Streamlit app in your browser.
   - Use the sidebar to upload a video file (supported formats: mp4, avi, mov, mkv).

3. **View object detection results:**
   - The uploaded video will be processed frame by frame.
   - Detected objects will be displayed with bounding boxes and class labels.
   - The processed video frames will be shown in real-time in the app.

## Code Explanation
### Imports and Model Loading
The project uses essential libraries such as Streamlit for the web application, OpenCV for image and video processing, NumPy for numerical operations, and Ultralytics YOLO for the object detection model.

### Generate Random Colours for Class List
Random colors are generated for the class list to visually differentiate detected objects.

### Streamlit App
The Streamlit app includes a sidebar for uploading video files and a main window for displaying the video with detected objects in real-time. The application processes each frame of the video, performs object detection using YOLOv8n, and draws bounding boxes and class labels on the video frames.

### Real-Time Object Detection
The application continuously captures video frames, performs predictions using the YOLOv8n model, and displays the results in real-time. Bounding boxes are drawn around detected objects, and class labels with confidence scores are displayed.

## Credits
This project uses the following libraries:
- **Streamlit** for creating the web app.
- **OpenCV** for image and video processing.
- **NumPy** for numerical operations.
- **Ultralytics YOLO** for the object detection model.

## Additional Notes
- You can adjust the confidence threshold in the code to filter out less confident detections.
- Ensure the COCO class names file (`coco.txt`) is correctly placed and accessible.
- The project demonstrates basic object detection and can be extended with more advanced features, such as tracking, handling multiple video formats, and improving the UI.

Feel free to fork this repository, contribute, or report any issues. Thank you for checking out this project!
