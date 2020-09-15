# GoKartProject

This project aims to design a control circuit that controls a current signal coming from Go-Kart external circuitry.
The controller board controls a Driver Board that is then interfaced a Power Circuitry Board that then powers a 24V DC motor. 
The control board is based on the design of a fixed frequency current mode controller UC3843. This conroller board works by 
comparing throttle current (Idemand) with the motor current (Imeasured) that is read a current sensor (LEM HAIS 150P).
