# humanoid
A female mobile robot that can do multilingual natural conversation, basic hand gestures, move around via wheels and identify known persons.

This robot uses RaspberryPi5 as it's brain that governs the working of all other components within the system.The brain is implemented via ROS2 Kilted Kaiju Framework within a docker container with a very moduler design. It uses PiperTTS for text to speech synthesis, Vosk for speech to text converison, OpenCV for Image Processing, ChatGPT API Key for natural conversations.The robot is typically divided into several individual nodes each handling different parts of the humanoid robot.

Such as: 
1. Eyes node handles the webcam for capturing live images
2. Ears node continously listen for user commands
3. Hands node deals with robot's hands
4. Legs node deals with locomotion of robot
5. Mouth node is responsible for speaking sentences and etc.

# Features
1. Natural conversation achieved via ChatGPT API
2. Recognizes Commands and perform corresponding acions. for ex: "move forward -> robot will move forward until said stop"
3. Hide&Seek Feature : User can say something like " find michael " and the humanoid moves in a specified protocol and searches for the face of michael and if found then it takes him to the original positon.
4. Can do basic hand gestures like namaste, hello etc
5. It can move in forward, backward, left and right.
6. It avoids obstacles in front from hitting while moving and stops until the obstacle is removed from its path.
7. It detects pits in ground while moving and stops at the moment it detect there is a pit in ground and doesn't move forward.

# Components used
1. Raspberry Pi 5 with 4GB RAM
2. Arduino Uno
3. Arduino Nano
4. MG995 Servo motors, QTY: 8
5. SG90 Servo motors, QTY: 4
6. MG90S Servo motor, QTY: 1
7. L298N Motor Driver
8. Jhonson Gear Motor, QTY: 2
9. Jumbo Wheels, QTY: 2
10. Caster Wheels, QTY: 2
11. UltraSonic Sensors HC-SR04, QTY: 2
12. 12V, 7AH Lead Acid Battery with Charger
13. 5V Relay
14. 12V Buzzer
15. 2 Speakers
16. PAM8403 with Bluetooth module
17. 128GB SSD
18. USB 3.0 TO SATA Adapter
19. Battery Level Indicator module
20. LM2596 Buck Converter, QTY: 2
21. XL4015 Buck Converter, QTY: 2
22. 300W DC-DC Step down buck converter
23. FUSE: 5A, 10A
24. 12V DC Fan