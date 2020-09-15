# ENEL471 - Go Kart Project

## Description
This project aims to design a control circuit that controls a current signal coming from Go-Kart external circuitry.
The controller board controls a Driver Board that is then interfaced a Power Circuitry Board that then powers a 24V DC motor. 
The control board is based on the design of a fixed frequency current mode controller UC3843. This conroller board works by 
comparing throttle current (Idemand) with the motor current (Imeasured) that is read a current sensor (LEM HAIS 150P).

## Requirements
###  Design Constraints (essential for real life limitation for Go Kart electrical vehicles)
- Forwad motor current must not exceed 350A. The current-time area above 150A msut not be exceed for more than 100 Amp-seconds.
- Reverse motor current must not exeed 100A.
- Average forward motor currrent must not exceedd 150A.
- no MOSFET can be switched faster than 5kHz.
### Note: Violation of Deisgn Constraints will result in a 5-second shutdown.

## Important
- The PWM signal which the deiver uses to switch the MOSFETS.
- The shutdown control S\D\, which disables the MOSFET diver chip.
- The 24V DC supply from which all pwer supplies must be derived.
- The current sensor header connections.

## Goals
### Successfully Producing a PWM using UC3843 chip
* Voltage swing of 5V (referenced to GND).
* Rise and fall times < 1us.
* A PWM switching frequency of 2.5kHz+-10%.
### A PWM that is controllable via throttle.
### Implementation of a fixed current mode control.
### Throttle sets average current and you limit aveage forward current to <150A, peak forward current to <350A and reverse current to <100A.

## Contributers
> - Hassan Alhujhoj
> - Abdullah Naeem 
> - Daniel Page