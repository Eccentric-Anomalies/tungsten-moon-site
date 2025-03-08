---
title: Home
layout: home
nav_order: 1
usemathjax: true
---
![Tungsten Moon landscape](/assets/images/banner.jpeg)
# TUNGSTEN MOON

In 1988, NASA found a wormhole that led to a remote star with a single planet. A gas giant. Orbiting the planet was a single moon made of solid metal. A Tungsten Moon.

A top-secret mission to the tungsten moon ended in 1996. The wormhole collapsed, but not before the entire mission crew escaped and returned to Earth. All, except for one astronaut, stranded, alone on the Tungsten Moon.

As a mission specialist, you were never trained to be a pilot. Learn to fly the single-seat SkyDart. Explore 1 million square kilometers of barren, lifeless terrain. Gather fuel, food, water, and resources to stay alive, waiting and hoping the day will come when you will be rescued: the day you will finally go home. 

## Demo Version

[Install The Demo On Steam](https://store.steampowered.com/app/3104900/Tungsten_Moon/){: .btn .btn-green }
[Download The Demo From Github](https://github.com/Eccentric-Anomalies/Tungsten-Moon-Demo-Releases/releases/tag/v1.0.0){: .btn .btn-blue }
[Read the Flight Manual](https://tungstenmoon.com/docs/manual/intro.html){: .btn .btn-purple }

The [Tungsten Moon Demo]({% link docs/manual/intro.md %}) is available for Windows and Linux and support both desktop and VR with keyboard or XBOX/PS game controller inputs in either mode. You can also set up PC analog joysticks or other flight sim hardware from inside the game. VR hand controllers support grabbing handles and pushing buttons (Vive/Quest tested).

# More About The Game

## The SkyDart

Manufactured by a little-known, defunct aerospace division of the old American car manufacturer, the AMC SkyDart is a single-seat utility/logistics spacecraft. With a delta-v capability of over 1400 m/s, the SkyDart can make point-to-point flights covering the entire surface of the tungsten moon.

The SkyDart uses a pressure fed, variable throttle, $N_2O_4/MMH$ hypergolic bipropellent engine, similar to the Space Shuttle OMS (orbital maneuvering system) engines, with a specific thrust of 300 seconds. Maximum thrust is 20 kN, and minimum thrust is 2 kN. Refueling can be automatically performed on the ground, at landing pads equipped with the necessary equipment.

SkyDart carries a maximum total fuel load of 2500 kg, and has an empty weight of 2500 kg, which are roughly equivalent to the specs of the old Apollo lunar module ascent stage.

## Instruments

SkyDart has two principal instruments: a ground radar and an inertial measurement unit.

The radar system has a range of 2000 meters and measures height above terrain and vertical velocity (rate of altitude change). Using the Doppler effect, the radar also computes a horizontal speed when the spacecraft is within 45 degrees of vertical. The horizontal speed is fed into a cross-pointer indicator to give the pilot a visual indication of the horizontal speed and direction. Radar system displays and readouts are located on the right-hand side of the cockpit windows.

The inertial measurement unit (IMU) has a three-axis gyroscope and accelerometer package that detects acceleration and the axis and magnitude of any spacecraft rotation. The gyro system can even measure the rotation of the moon when SkyDart is parked on the ground. From the rotation, it can infer which direction the spacecraft is facing, and its latitude.

Once calibrated on the ground, the IMU can be used to set the orientation of the artificial horizon “nav ball” indicator on the left-hand side of the cockpit windows. In flight, the IMU updates its estimate of the spacecraft altitude above a baseline, and its speed, relative to the center of the moon.

## Ground Beacons

Certain ground-based installations transmit beacons signals are detected by the SkyDart radio. Information on range and bearing to beacons is available in the flight computer and can be used to drive the cross-pointer display as an aid to navigation.

## Packet Radio System

Certain ground-based installations act as repeaters in a global data packet forwarding network. The SkyDart pilot can request and receive information from ground stations or other spacecraft anywhere on or above the moon. 

## Flight Computer

SkyDart uses a 68000-based, 16-bit microcomputer for navigation and autopilot functions. Applications are programmed using the Forth language. Built-in control and measurement functions include:
* Attitude stabilization
* Lateral drift stabilization
* Vertical rate stabilization
* Orbital calculations, including apoapsis and periapsis altitudes, and projected distance and direction to ground impact.
* Great circle distance, and bearing, from liftoff point.

The Forth control programs and flight parameters are accessible to the pilot and can be extended.


