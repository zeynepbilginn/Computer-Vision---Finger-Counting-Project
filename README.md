## Finger Counting Application

This Python application utilizes computer vision techniques to count the number of fingers shown in front of a camera in real-time. It segments the hand from the background and analyzes its contour to determine the number of fingers.

### How It Works

1. **Background Subtraction:** The application initially captures and processes the background to isolate moving objects, which in this case, is the hand.

2. **Hand Segmentation:** Using background subtraction, the hand is segmented from the rest of the frame by identifying the contours of the hand.

3. **Finger Detection:** Once the hand is segmented, the application calculates the convex hull of the hand and determines the number of fingers by analyzing specific features such as the number of convexity defects and their locations.

4. **Real-Time Display:** The application provides real-time feedback by displaying the segmented hand and the count of fingers directly on the screen.

### Dependencies

- OpenCV: Used for image processing tasks such as background subtraction, contour detection, and image manipulation.
- NumPy: Utilized for numerical operations and array manipulations.
- Scikit-learn: Specifically, the `pairwise` module is used to compute pairwise distances between points in two sets.



