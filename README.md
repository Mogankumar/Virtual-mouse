# Virtual-mouse

This project implements a Virtual Mouse using computer vision and hand gesture recognition. It leverages a webcam to detect hand landmarks and performs actions such as moving the cursor, clicking, scrolling, and taking screenshots, making it a touch-free alternative for controlling a computer.

**Features**
1. Move Cursor: Control the mouse pointer using the index finger.
2. Click: Perform a left-click by pinching the index and middle fingers together.
3. Scroll: Scroll up or down using specific hand gestures.
4. Take Screenshots: Capture the screen by making a designated gesture.
5. Real-time FPS Display: Displays the frame rate (FPS) of the video feed for performance monitoring.

 **How It Works**
1. Hand Detection:
	•Uses a hand tracking module to detect landmarks of the hand.
	•Identifies the index finger, middle finger, and thumb for specific gestures.
2. Gesture Recognition:
	•Single Index Finger Up: Moves the cursor on the screen.
	•Pinch Gesture: Performs a left-click when the distance between the index and middle fingers is less than a threshold.
	•Thumb and Index Finger Gesture: Scrolls up or down.
	•Specific Gesture: Captures a screenshot.
3. Mouse Control:
  	•Cursor movements are smoothed for better accuracy.
  	•Mouse control and clicks are performed using the autopy and PyAutoGUI libraries.

**Example Gestures**
   
**Gesture	                                Action**
Index finger up	                        Move cursor
Index + Middle fingers pinched	        Left click
Thumb + Index	                          Scroll up/down
All fingers out (specific gesture)	    Capture screenshot
