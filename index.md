---
title: Home
layout: home
nav_order: 1
usemathjax: true
---
![Tungsten Moon landscape](/assets/images/banner.jpeg)
# TUNGSTEN MOON

In 1988, NASA found a wormhole that led to a remote star with a single gas giant planet. Orbiting the planet was a single moon made of solid metal: A Tungsten Moon.

Your new life on the Tungsten Moon begins in deep mystery. You wake up in a spacecraft that you have never flown 
before, with a mission so secret that even you aren't sure what it is. Someone is sending you messages to help
you get off the ground, but who are they and what do they really want from you?

Survival is the most important task. Learn to fly the SkyDart spacecraft, with a minimum
of instruments. There is no tech on board better than what you would expect from a bargain-basement spacecraft
manufactured by a second-rate US auto maker. Find fuel, deliver Tungsten ore, and stay alive, no matter what
occurs!

## Demo Version

[Install The Demo On Steam](https://store.steampowered.com/app/3104900/Tungsten_Moon/){: .btn .btn-green }
[Download The Demo From Github](https://github.com/Eccentric-Anomalies/Tungsten-Moon-Demo-Releases/releases){: .btn .btn-blue }
[Read the Flight Manual](https://tungstenmoon.com/docs/manual/intro.html){: .btn .btn-purple }

The [Tungsten Moon Demo]({% link docs/manual/intro.md %}) is available for Windows and Linux and support both desktop and VR with keyboard or XBOX/PS game controller inputs in either mode. You can also set up PC analog joysticks or other flight sim hardware from inside the game. VR hand controllers support grabbing handles and pushing buttons (Vive/Quest tested).

# More About The Game

## The SkyDart

Manufactured by a little-known, defunct aerospace division of the old American car manufacturer, the AMC SkyDart is a single-seat utility/logistics spacecraft. With a delta-v capability of over 1400 m/s, the SkyDart can make point-to-point flights covering the entire surface of the tungsten moon. Theoretically. Survival is always the
catch.

The SkyDart uses a pressure fed, variable throttle, $N_2O_4/MMH$ hypergolic bipropellent engine, similar to the Space Shuttle OMS (orbital maneuvering system) engines, with a specific thrust of 300 seconds. Maximum thrust is 20 kN, and minimum thrust is 2 kN. Request fuel from any ground facility with refueling ability.

SkyDart carries a nominal maximum fuel load of 2500 kg, can carry an overload of an additional 1600 kg or
a Tungsten ore payload of up to 2000 kg (but not both at the same time!). With an empty weight of 2500 kg, 
SkyDart is in a performance category similar to the previous decade's Apollo Lunar Module.

## Instruments

SkyDart has two principal instruments: a ground radar and an inertial measurement unit.

The radar system has a range of 2000 meters and measures height above terrain and vertical velocity (rate of altitude change). Using the Doppler effect, the radar also computes a horizontal speed when the spacecraft is within 45 degrees of vertical. The horizontal speed is fed into a cross-pointer indicator to give the pilot a visual indication of the horizontal speed and direction. Radar system displays and readouts are located on the right-hand side of the cockpit windows.

The inertial measurement unit (IMU) has a three-axis gyroscope and accelerometer package that detects acceleration and the axis and magnitude of any spacecraft rotation. 

Once calibrated on the ground, the IMU can be used to set the orientation of the artificial horizon “nav ball” indicator. 

## Packet Radio System

Certain ground-based installations act as repeaters in a global data packet forwarding network. The SkyDart pilot receives short messages from ground stations or other spacecraft anywhere on or above the moon. 

## Flight Management System (FMS)

SkyDart uses a 68030-based, 16-bit microcomputer for on-board computing. Applications are programmed using 
the Forth language. Built-in FMS functions include:
* Landing gear diagnostics
* Landing pad service comms, including requests for fuel and ore transfer, and landing gear repairs.
* Storing and viewing messages received via Packet Radio.
* Ship's chronometer, including an up/down stopwatch function for timing engine burns.

