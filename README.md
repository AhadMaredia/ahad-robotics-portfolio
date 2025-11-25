Robotics Portfolio – Ahad Maredia

Welcome to my Robotics Portfolio for my ITAI Robotics course.
This repository documents all my robotics work during the semester, including assignments, robot experiments, presentations, and my final project using the SunFounder PiCar-X.

##  Table of Contents

About Me

PiCar-X Projects

Assignments

AI Conference Presentation

Final Project – Ball-Following Robot

Future Work

##  About Me

I am a robotics and AI student passionate about intelligent systems, autonomous vehicles, and applied machine learning.
This portfolio showcases the robotics concepts, coding projects, and hands-on experiments I completed throughout the course.

##  PiCar-X Projects

This semester, we worked extensively with the SunFounder PiCar-X, a Raspberry Pi–powered autonomous robot.

1. Movement, Steering, & Basic Controls

We tested 13 commands that verified:

Forward / reverse driving

Turning left / right

Motor calibration

Camera servo movement

Speed control

Folder: /picar-x/movement_tests/

2. Object Detection

Using OpenCV and the PiCar-X camera, we ran experiments detecting objects in real time.

Folder: /picar-x/object_detection/

3. Face Tracking (Camera-Only Movement)

We used facial detection so the camera head (pan/tilt servos) tracked faces while keeping the robot body stationary.

Folder: /picar-x/face_tracking/

4. ChatGPT API Voice Assistant

I integrated the OpenAI API so we could speak to the PiCar-X and receive voice/text responses back from ChatGPT.

This allowed hands-free interaction with the robot.

Folder: /picar-x/chatgpt_api_integration/

5. SunFounder Controller App

We connected the PiCar-X to the official SunFounderController mobile app to remotely control driving, camera movement, and speed.

Folder: /picar-x/sunfounder_controller/

##  Assignments

All class assignments are included in the assignments/ folder:

✔️ Raspberry Pi 5 Presentation

(Raspberry_Pi_5_Presentation.pptx)

✔️ Robot Sensors One-Pager (Boston Dynamics Spot)

(Robot_Sensors_OnePager_Spot.docx)

✔️ Robotics Glossary

(Robotics_Glossary_Ahad_Maredia.docx)

##  AI Conference Presentation

I attended and presented the PiCar-X at an AI Conference held on campus.

I demonstrated:

The PiCar-X hardware

Its autonomous capabilities

Object & face detection

ChatGPT integration

Potential future uses (education, prototyping, research)

This experience helped me practice technical communication with teachers, administrators, and industry professionals.

Folder: /images/conference/ (Add photos here)

##  Final Project – Ball-Following “Fetch Mode” PiCar-X

For my final project, I am building a system where the PiCar-X behaves like a dog chasing a ball.

Goal

Have the robot detect a ball → follow it → keep moving toward it as it rolls or moves.

My Approach
1. Capture Training Data

The PiCar-X camera takes grayscale images

Images are labeled as “ball present” or “no ball”

2. Computer Vision + ML

Options include:

Thresholding + contour detection

Color detection

Tiny CNN model for grayscale ball detection

Or even a small YOLO-based model

3. Tracking Logic

Once the ball is detected:

If the ball is centered → drive forward

If ball is left → turn left

If ball is right → turn right

If ball disappears → stop or search

Folder: /picar-x/final_project_ball_following/
