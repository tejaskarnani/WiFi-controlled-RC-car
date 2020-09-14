# WiFi-controlled RC car

### Description
We wrote a program that turns your raspberry pi into a Radio controller for RC cars without any additional hardware. Using this project, you can drive any cheap toy-grade RC car programatically with your raspberry pi.
Note that running this program turns your pi into a rather powerful radio transmitter.

### Components Required
<img src="https://github.com/tejaskarnani/WiFi-controlled-RC-car/blob/master/Required%20Components.jpeg" height="640" width="480" rotate="90">

* 4x4 drive RC car
* Raspberry pi 3, or higher
* L293D motor driver shield for Arduino.
* Jumper wires - Female to Female, and Female to Male
* Pi Camera

### Connections
![alt text](https://github.com/tejaskarnani/WiFi-controlled-RC-car/blob/master/Connections.png)

## Steps to run
* _Installing files in the repository (change)_
* On your raspberry pi, open two terminal shells to run simulaneously. It is also helpful to open a browser window at this time (used later)
* Navigate to the folder pi_rc_master and type **sudo -s**. Then in the prompt, type **./pi_pcm -v**. 
* In the second terminal shell, while the first one is running, after navigating to the folder, run the host files in python by using **python3 host_files.py**.
* This command returns two URLs. Copy the first, and paste it in the browser window. The browser may return a warning, saying that the page is not secure. Override this by going to 'advanced' and then clicking on 'Go to' address.
* In the list of files, go to **watch.html** to see a preview of the video from the Pi Camera.
* Go back to the list of files, then to **control.html**. Scroll down to the option to "Select JSON Parameter file". The files in the repository have 4 parameter files. You need to figure out which JSON works with your choice of Motor Driver and RC Car. For us, it was ***jsbr-ford-mustang-27mhz.json***
* After loading the right parameter file, try controlling the car using the buttons on **control.html**. 

## Who needs remote controllers?


### Disclaimer
Do not use this code unless you understand what it does, what frequencies it might interfere with, what frequencies are allowed, what is legal in your country, etc. I assume no responsibility for your actions or for any problems running this program may cause.

## Credits
bskari

