## How to run

To launch the code, you just have to sue the commands `roslaunchlineFollowerVibhu linemission.launch model:=waffle` to launch the simulation and then you have to use `rosrun lineFollowerVibhu follower.py` to tell the robot to start following the line.

## How it works
Much like the example from class, the image is processed in the image_callback function, which converts the image so that it can be used by cv2 and then it changes the format to HSV to set up the band that is going to be used to determine where the yellow line is on the ground. After it sets up the band that the robot is going to look it, it also sets up a centroid, a red dot that will follow the yellow line. If the centroid is not in the center, the movement commands for the robot will be updated to center it again, meaning that if there is a turn in the line and the centroid turns to follow it, the robot will then turn to follow the centroid.

## Links for the recording
https://drive.google.com/drive/folders/10wmaOTa7z6PeCqV1ytEvfPQ0SPyEa6O7?usp=sharing
