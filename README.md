# Hexapod-demo

This repo. is dedicated to the hexapod personal project used for skill show off and demonstration.

![alt text](https://github.com/xapha/Hexapod-demo/blob/main/hexapod.png "intro figure")

## Intro :

The objectives of the platform are:
- Fully 3D printed
- Only low cost digital servos (18 used in this prototype)

Tools used to create the prototype:
- Fusion 360
- Ultimaker Cura
- Simplify 3D

Machinery:
- 3d printer Creality CR-10

Components:
- SSC 32U servo controller
- Raspberry Pi 2B
- Battery (Nimh 4400 mAH)
- Tension regulator (5v)
- Servos : TowerPro MG996R x 18
- IMU shield for Rpi

## Materials:

- Motion video (remote controlled) :
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/dWkvSa4oxTY/0.jpg)](https://www.youtube.com/watch?v=dWkvSa4oxTY)
- 3D model reference in repo files

## Robot capabilities:
- Control : remote controlled or autonomy 
- Motion : Wave motion (5 legs in contact with the ground at the same time), Ripple motion (4 legs in contact with the ground at the same time), Tripod motion (3 legs in contact with the ground at the same time)
- Motion composition : can perform translation and rotation in unique movement or in composition
- Elevation variation : can change its base elevation to adapt to the terrain while moving or standing
- Orientation control : use IMU data to specifiy each legs height to keep the same orientation while moving
- Indirect detection : void, obstacle : use IMU data to detect the lack of surface to walk on and obstacle through signal processing
- Mapping : map the environement based on previous location and motion: Obviously this is drifting a lot since no loop closure system is used, SLAM for the next one.
- 45 min autonomy without additional modules
