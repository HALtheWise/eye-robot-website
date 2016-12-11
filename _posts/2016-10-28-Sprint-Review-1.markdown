---
layout:     gslides
title:      Sprint 1
# author:     Eric
tags: 		
subtitle:  	Pivoting into Telepresence
category:   sprint-review
---
<!-- Start Writing Below in Markdown -->



<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vRMl08x10zIRdb5I1dDOkngbKSJFNGaBwYYbRmvsZ6HnpTv9-92c4wbgG4tJ7PpTdfe0Ze8WAMCBRoa/embed?start=false&loop=false&delayms=3000" frameborder="0" width="1170" height="681" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

<p> As of sprint one, our goal was to create an immersive experience where, by putting on a google cardboard viewer, a user could look through the eyes of a tiny robot. </p>
<p>As such, we defined our minimum viable product as a mobile platform that streamed video from a single camera to a google cardboard virtual reality viewer. We also wanted to ideally make our experience truly immersive , provide web access, and have some sort of a manipulator on the robot that the user could control.</p>
<p>For our first sprint, we recognized that one of our highest areas of technical risk was the connections between the many pieces of software and hardware that would be needed to control eye-robot. In order to buy down this risk, we sought to build a system that demonstrated all of the key hardware and software connections we'd need. </p>
<p>As of sprint one, our planned controls system consisted of a phone running a cardboard app that displayed video mjpg streams from two raspberry pi board computers on the robot and streaming accelerometer data that could be used to control the robot to one of the raspberry pis.We planned to use cameras purpose built to work with the raspberry pi hardware. The rasberry pi that recieved control data would communicate robot commands to an arduino via seria, which in turn would control the servos that moved the head and the motor controller that provided power to the drive motors.</p>
<p>By the end of the first sprint, We had an android app on the phone displaying an mjpeg stream from a rasberry pi connected to a USB webcam. We also had the robot controlled via arduino, though instead of controlling the robot via serial from a raspi we used a python script on a computer to generate the robot commands. </p>
<p>Through the course of our sprint, we learned that the google cardboard and immersive aspects of our project would be the hardest to implement. Performance limitations on the phone made mjpeg streaming at high framerates a difficult problem to solve, and the learning curve to use the google caradboard API was incredible steep. We also learned that we had to plan for our team member avaliability in advance so we weren't missing team members through our crunch time, and make sure that we were all working towards our goals at all times. </p>


<!-- [Link to Google](https://www.google.com) -->
<!-- ![Image embed]({{ site.baseurl }}/img/Logo_Fairy_Tail_right.png) -->
