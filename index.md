---
title: Home
layout: home
nav_order: 1
usemathjax: true
---
![Tungsten Moon landscape](/assets/images/banner.jpeg)

[Install The Demo On Steam](https://store.steampowered.com/app/3104900/Tungsten_Moon/){: .btn .btn-green }
[Read the Flight Manual](https://tungstenmoon.com/docs/manual/intro.html){: .btn .btn-purple }
[Contact the Developer](/contact/){: .btn .btn-blue }

# TUNGSTEN MOON

In 1988, astronomers found a wormhole that led to a remote star with a single gas giant planet. Orbiting the planet was a moon of solid metal: a Tungsten Moon.

Your new life on the Tungsten moon begins in deep mystery. You begin in a spacecraft that you have never flown before, with a mission so secret that even you don't know what it is. Someone is sending you messages to help you get started, but who are they, and what do they really want from you?

Survival is the most important problem. Learn to fly the Sky Dart spacecraft with a minimum of instruments. There is no tech on board better than what you would expect from a bargain-basement spacecraft manufactured by a second-rate US auto maker. Find fuel, deliver tungsten ore, and stay alive, no matter what occurs!


## Demo Version

The [Tungsten Moon Demo]({% link docs/manual/intro.md %}) is available for Windows and Linux and support both desktop and VR with keyboard or XBOX/PS game controller inputs in either mode. You can also set up PC analog joysticks or other flight sim hardware from inside the game. VR hand controllers support grabbing handles and pushing buttons (Vive/Quest tested).

## Press Kit

See the [Tungsten Moon Press Kit](https://steamkit.dev/press/tungsten-moon).

# More About The Game

## The Sky Dart

Manufactured by a little-known, defunct aerospace division of an old American car manufacturer, the AMC Sky Dart is a single-seat utility/logistics spacecraft. With a delta-v capability of over 1400 m/s, the Sky Dart can make point-to-point flights covering the entire surface of the tungsten moon. Theoretically. Survival is always the catch.

The Sky Dart uses a pressure-fed, variable throttle, $N_2O_4/MMH$ hypergolic bipropellant engine, similar to the Space Shuttle OMS (orbital maneuvering system) engines, with a specific thrust of 300 seconds. Maximum thrust is 20 kN, and minimum thrust is 2 kN. Request fuel from any ground facility with refueling ability.

Sky Dart carries a nominal maximum fuel load of 2500 kg and can carry an overload of an additional 1600 kg or a tungsten ore payload of up to 2000 kg (but not to exceed the maximum takeoff weight of 6250 kg!). With an empty weight of 2500 kg,
Sky Dart is in a performance category similar to the previous decade's Apollo Lunar Module.


## Instruments

Sky Dart has two principal instruments: a ground radar and an inertial measurement unit.

The radar system has a range of 2000 meters and measures height above terrain and vertical velocity (rate of altitude change). Using the Doppler effect, the radar also computes a horizontal speed when the spacecraft is within 45 degrees of vertical. The horizontal speed is fed into a cross-pointer indicator to give the pilot a visual indication of the horizontal speed and direction. 

The inertial measurement unit (IMU) has a three-axis gyroscope and accelerometer package that detects acceleration and the axis and magnitude of any spacecraft rotation. Once calibrated on the ground, the IMU can be used to set the orientation of the artificial horizon indicator.

Radar and IMU system displays and readouts are located on the right-hand side of the cockpit window.

## Packet Radio System

Certain ground-based installations act as repeaters in a global data packet forwarding network. The Sky Dart pilot receives short messages from ground stations or other spacecraft anywhere on or above the moon. 

## Flight Manual

Sky Dart comes equipped with a comprehensive in-cockpit flight manual, including:
* System overview and specifications
* Systems performance, including range and flight duration charts at different weights
* Description of pilot instruments and controls, including hover autopilot
* Simulation control methods, such as game controller buttons, PC keyboard, etc.

## Flight Management System (FMS)

Sky Dart uses a 68030-based, 16-bit microcomputer for on-board computing. Applications are programmed using the Forth language (customizable by the player). Built-in FMS functions include:
* Landing gear diagnostics
* Landing pad service handles requests for fuel, ore transfer, and landing gear repairs.
* Storing and viewing messages received on the Packet Radio system.
* Ship's chronometer, including an up/down stopwatch function for timing engine burns.
