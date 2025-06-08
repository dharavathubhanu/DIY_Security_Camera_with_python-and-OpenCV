# Motion Detection with Beep Alert using OpenCV
This Python project uses your computer’s webcam to detect motion in real-time. When significant movement is detected, it plays a beep sound as an alert using the winsound module. Ideal for building a simple home security system or motion-triggered notifier.

# Features
Real-time motion detection using frame differencing
Plays a beep alert (500 Hz, 100 ms) on detecting motion
Filters out small or insignificant movements (like light flicker or shadows)
Runs entirely on your local machine with no need for internet or external hardware

# How It Works
1. Captures two consecutive frames from the webcam.
2. Calculates the absolute difference between the frames to detect changes.
3. Converts the difference to grayscale and applies thresholding to highlight motion.
4. Contours are extracted from the binary image to identify moving regions.
5. If the area of any contour exceeds a threshold (5000 px), it triggers a beep.

# Requirements
pip install opencv-python
Note: winsound is a built-in module available on Windows. For other platforms, alternative sound libraries may be required.

# How to Run ?
1. Make sure your webcam is connected.
2. Run the script:
python security_cam.py
3. A window titled "Security camera" will display areas of detected motion.
4. If significant motion is detected, your system will beep.
5. Press ESC to exit the program.



