# Workflow
This program is based on a technique known as gaussian background subtraction. This technique is widely used for detecting moving objects with a steady camera.
Background subtraction creates a mask representing the background of a frame (the static part of an image) and for each frame, it subtracts the previous one.
Let’s have a gentle overview of the main two steps on how this algorithm works:
  Background Initialization: In this first step, a model of the background is calculated by freezing the first frame.
  Update: In this second step the next frame is being subtracted from the previous, hence, if a change (a movement) happened between the     two frames, the difference of the frames will reflect the change which can be market by applying a filter.

# To Run follow these steps:
  1.)Run `python motion_heatmap.py `
  2.)If you want to use another video change the path in `motion_heatmap.py` in the `main()` function.

# Requirements
To run this script you will need python 3.6+ installed along with OpenCV  3.3.0+ and numpy.
Make also sure to have installed the MOG background subtractor by running:

`pip install opencv-contrib-python`

# Enjoy!

# Acknowledgement
https://towardsdatascience.com/build-a-motion-heatmap-videousing-opencv-with-python-fd806e8a2340
