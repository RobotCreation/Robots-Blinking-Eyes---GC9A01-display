# Robots-Blinking-Eyes---GC9A01-display
This is the robot's blinking eyes using two GC9A01 1.28-Inch Round LCD TFT Display

![Screenshot 2024-08-13 112239](https://github.com/user-attachments/assets/d4d73b5c-27c2-40ac-8f5b-01d5ba31416f)

The Robot eyes were originally based on the Uncanny eyes found on internet which uses ESP32. 
For simplicity Raspberry Pico or RP2040 was used but since these processors don’t have enough memory, the display of the eyes were too slow and the following solution seems to work.
The solution is based on writing the BMP image to the display buffer as the processor boots and then just point to a part of the display that you want the pupils to be and this has the effect of eyes blinking.
ESP32-CAM could also be used to provide the XY coordinates of the person in front and send the location to the Pico, so that the eyes follow you around the room.
The current code displays the eyes in random positions. This was chosen as the Robot head is following you across the room.  
