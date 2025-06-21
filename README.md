🎨 Virtual Paint App using MediaPipe and OpenCV
This is a real-time hand tracking paint application built using Python, OpenCV, and MediaPipe. It allows users to draw on a virtual canvas using hand gestures captured via a webcam. The user selects different colors by hovering their index finger over on-screen color buttons and starts/stops drawing by performing a pinch gesture (thumb touching index finger).

✨ Features
1.👋 Detects and tracks one hand using MediaPipe

2.🎨 Lets you draw with your index finger using virtual colors

3.🟡 Color selection via on-screen buttons (Blue, Green, Red, Yellow, Purple, Black)

4.🖐️ Drawing activated by pinching (thumb and index finger close together)

5.🔲 Shows bounding box around the hand and fingertip trails

6.📷 Displays two windows:

  -"final img": live feed with overlays

  -"empty img": virtual canvas with just the drawing

7.⚡ Real-time FPS calculation and display

8.🧹 Press C key to clear all drawings

9.❌ Press Q key to quit

🧰 Libraries Used
1. OpenCV (cv2) — for video capture and drawing on images

2. MediaPipe — for hand landmark detection

3.NumPy — for managing drawing arrays

4. Math — for distance calculation

5. Time — for FPS calculations

🖌️ How It Works
1. Hand Detection:
Uses MediaPipe’s Hands model to track up to 1 hand and detect 21 landmarks in real-time.

2. Drawing Gesture:
Drawing is enabled only when the user brings the thumb tip and index tip close together. This is determined using the distance between them.

3. Color Selection:
When the index fingertip hovers over a colored circle (like Blue, Green, etc.), it activates that color for drawing.

4. Drawing on Canvas:
All drawings are stored as polylines in a NumPy array and rendered continuously onto a blank canvas image.

