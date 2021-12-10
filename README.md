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

Next open your python idle and install the necessary modules.

make sure to connect your arduino to your PC and specify the correct USB slot. To get the name of your USB slot  
