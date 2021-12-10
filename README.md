# Robotic-car-with-object-detection

This is project based on sustainable development goal 6 (SD-6) where the robot will go and pick any kind of waste paper or waste plastic in the ground, store it in a container and make sure that the surronding is clean.

Here the project is divided into two parts -> the car and the robotic arm.
1. The car's job is to go near the waste plastic and this is done by using a CMOS camera. Here the opencv object detection is used.
2. The robotic arm part is to pick the detected object.

Now the above parts and modules are combined and if the object is detected it will go near near the object and the arm will pick the object.
There is a sample video demo in the repo.

Now the components needed:
1. arduino uno
2. car chasis
3. robotic arm
4. servo motors x4
5. L293d motor driver
6. separate power supply for running the car
7. ultra sonic sensor (if needed for calculating the distance)

![20211121_225006](https://user-images.githubusercontent.com/91727830/145608787-2d8a3b0c-6a76-4780-bec0-fcf36b49cb6b.jpg)

Now upload the standard pyfirmata to your arduino -> Refer youtube videos for pyfirmata. A basic intro is that pyfirmata is used to run the robot using python. NOTE: some setting are to be changed inorder to upload the pyfirmata to the arduino (Refer youtube).

Next open your VS Code (recommended) and install the necessary python modules.

Make sure to connect your arduino to your PC and specify the correct USB slot. To get the name of your USB slot connect the arduino to USB and go to Arduino IDE->Tools->Ports there you will get your USB port name.

Now open the main code movingcar.py and locate the terminal directory to the main code (movingcar.py) using cd (path). At the 199th line there is line copy that and paste that in VS Code terminal.
NOTE: if you want you can change the object class that the camera object want to detect in line 162.

now hit enter and It will take some time.

BOOM now the complete project is done and it is ready to detect and pick the objects.

Future project modification plan:-
1. The distance is pre-defined, so we can find the distance using ultrasonic sensor. But we are going to implement it using Object disstance method using the camera itself. YOLO distance calculation method.
2. The camera we are going to use is ESP32 cam which is a wifi cam instead of webcam.

# Sample video is uploaded in the repo.
