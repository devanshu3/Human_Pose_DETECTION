## Human_Pose_DETECTION
This Python program performs real-time human pose estimation using the MediaPipe library and OpenCV. It captures video frames from a video file or webcam, processes them for pose detection, and visualizes the detected pose landmarks on the frames. This program is useful for various applications, including fitness tracking, sports analysis, and gesture recognition.


## Prerequisites
Before running the program, you need to ensure that you have the required Python libraries installed: OpenCV (opencv-python) ,MediaPipe (mediapipe)
You can install these libraries using pip: pip install opencv-python, mediapipe


## Usage
The program can be used in two modes: video file mode and real-time webcam mode.

_Video File Mode_
#Open a video file (e.g., 'test_video.mp4')
cap = cv2.VideoCapture('test_video.mp4')
#Press 'q' to exit
if cv2.waitKey(1) == ord('q'):
    break
    
_Real-time Webcam Mode_

#Open the webcam (camera index 0)
cap = cv2.VideoCapture(0)
#Press 'q' to exit
if cv2.waitKey(1) == ord('q'):
    break

    
## Configuration
You can customize the program's behavior by modifying the following parameters in the code:
min_detection_confidence: Minimum confidence threshold for pose detection.
min_tracking_confidence: Minimum confidence threshold for pose tracking.
Resize frame dimensions: You can resize frames to a specific width and height for better performance.

#Example configuration
pose = mp_pose.Pose(min_detection_confidence=0.5, min_tracking_confidence=0.5)
frame = cv2.resize(frame, (350, 600))


## Keyboard Controls
Press 'q' to exit the program.


## Contact
Feel free to contact on queries or correction via *rawatdev0781@gmail.com* 
devanshu3
