pip install opencv-contrib-python

Use all.py file to run through various background subtraction algorithms (KNN, MOG, MOG2, GMG, CNT) using live feed as input
Use contor.py for contouring on motion detection
Use main.py for motion detection on live feed using mog2 as subtraction method with different conditions applied (delay, area, threshold)
To use webcam change the videopaths value to zero
You can use different demo cam video too.

Delay (-d) - Amount of time in seconds to delay the program before starting. 
        This is useful for if you need to set up the camera and get out of the way before execution.

Min Area (-m) - Minimum area in pixels difference to be considered actual motion. 
           This effects the overall sensitivity of the motion detector. Lowering the area will make the program much more likely to detect motion. 
           Should be used with caution as setting it too low will have the camera become overly sensitive to things such as background noise or scratches.

Thresh (-t) - The level of threshold intensity. 
         This can be useful for tweaking the program to run under different lighting conditions. 
         Increasing it will help it to run in particularly bright conditions, howeverleaving it as is should be sufficient for most use cases.

Video Path (-v) - Path to a video file you would like to run the program with. 
             Program defaults to using your device's default capture device.

To run the main file in cmd:
python 2main.py -t 90 -v "C:\Users\hi\Desktop\New folder (2)\night.mov"


For more cctv videos:  "http://backgroundmodelschallenge.eu/"
