---
layout:     post
title:      Electrical System
author:     Eric
# tags: 		design
subtitle:  	Some Short Description of Post
category:   design

published: true
---
<!-- Start Writing Below in Markdown -->

<!-- Table of Contents -->
<!-- 
* TOC
{:toc} -->

# Electrical system diagram
![Image embed]({{ site.baseurl }}/img/eye-robot-electrical.svg)

# Design approach
Our electrical system is driven by a requirement to provide large amounts of high-voltage power to the main drive motors (which operate at 12V) while maintaining a stable power supply at 5V for the control electronics. Additionally, the entire electrical system needed to be split between the lower body (which contains the power source, switching electronics, and motors) and the upper head, which needs to contain the camera and Raspberry Pi. 

To accomplish this, we powered the robot with two independent power sources:
- A large sealed lead-acid battery capable of powering the motors at stall current
- A USB battery pack providing 5V for the control electronics and servos

This split approach also allowed us to use the main power switch to disable only the large motors, which proved extremely convenient for testing purposes.

# Lessons learned
1. Have a power switch, it makes testing easier
1. Be careful about how much current you put through thin wires, particularly if the systems are sensitive to voltage drop
1. Place your electrical components on a single board to the extent possible, because it makes maintaince easier
1. Make sure your chassis is designed to grant easy access to the electrical components for emergency debugging


<!-- [Link to Google](https://www.google.com) -->
<!-- ![Image embed]({{ site.baseurl }}/img/Logo_Fairy_Tail_right.png) -->
