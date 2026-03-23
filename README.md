# 6-DOF Robotic Arm

A six degrees-of-freedom robotic arm controlled over Wi-Fi using an ESP8266.
Each joint is individually adjustable through a custom IoT dashboard built on
the Blynk platform.

## Control

The arm is controlled remotely via [Blynk](https://www.blynk.io/), with each
motor mapped to a separate slider/control in the app. This lets you position
every joint independently in real time over a local network or the internet.

## Stack

| Part | Details |
|---|---|
| Controller | ESP8266 |
| IoT Platform | Blynk |
| Control Method | Wi-Fi / Remote dashboard |
| Degrees of Freedom | 6 |

## How it works

The ESP8266 connects to the Blynk cloud and listens for input from the mobile
app. Each virtual pin corresponds to one motor, so moving a slider in the app
directly drives the respective servo on the arm.