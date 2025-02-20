# Hands-Free Mouse Control for Paraplegics and Paralytics

## Overview
This project provides a hands-free mouse control system for individuals with physical disabilities, such as paraplegics and paralytics, who cannot use traditional input devices. The system uses **facial landmark detection** and **eye/mouth movement tracking** to enable cursor movement and mouse clicks through facial gestures. Built with **Computer Vision** techniques and Python libraries like **dlib**, **OpenCV**, and **PyAutoGUI**, it offers a real-time, hardware-free solution.

---

## Features
- **Hands-free cursor control**: Move the cursor using head movements.
- **Facial gesture-based clicks**:
  - **Right Eye Wink**: Right-click.
  - **Left Eye Wink**: Left-click.
- **Mouth Gestures**:
  - **Mouth Open/Close**: Activate or deactivate mouse control.
- **Scroll Control**:
  - **Squinting**: Activate or deactivate scrolling.
  - **Head Movements**: Scroll up or down.
- **Real-time response**: Average response time of 15-20 milliseconds.
- **No additional hardware**: Works with a standard webcam.

---

## Technical Details
The system uses:
1. **Facial Landmark Detection**: Detects 68 facial landmarks using the **dlib library**.
2. **Eye Aspect Ratio (EAR)**: Detects eye blinks and winks.
3. **Mouth Aspect Ratio (MAR)**: Detects mouth opening and closing.
4. **Head Movement Tracking**: Tracks head pitch and yaw for cursor movement and scrolling.
5. **PyAutoGUI**: Moves the cursor and performs clicks.
6. **OpenCV**: Captures and processes real-time video from the webcam.
7. **Convex Hull**: Visualizes facial landmarks and detects facial features.

---

## How It Works
1. **Facial Landmark Detection**: The system detects the user's face and extracts 68 facial landmarks using the dlib library.

2.**Eye and Mouth Tracking**:

  2.1**Eye Blinks/Winks**: Detected using the Eye Aspect Ratio (EAR). A drop in EAR indicates a blink or wink.

  2.2**Mouth Open/Close**: Detected using the Mouth Aspect Ratio (MAR). An increase in MAR indicates an open mouth.

3.**Cursor Movement**: Head movements (pitch and yaw) are tracked to move the cursor in real-time.

4.**Mouse Clicks**:

  4.1 A right eye wink triggers a right-click.

  4.2 A left eye wink triggers a left-click.

5 **Scrolling**: Squinting activates scrolling, and head movements control the scroll direction.

---
## Conclusion

This project demonstrates the potential of Computer Vision and Human-Computer Interaction (HCI) to create accessible solutions for individuals with physical disabilities. By enabling hands-free control of a computer, this system empowers users to interact with technology in a way that was previously inaccessible to them.

---

