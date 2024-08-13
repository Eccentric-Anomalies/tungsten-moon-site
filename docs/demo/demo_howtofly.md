---
layout: default
title: How to Fly the Sky Dart
parent: Tungsten Moon Demo
nav_order: 3
usemathjax: true
---

# How to Fly the Sky Dart
Don't worry. It's only rocket science!

{: .no_toc }


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

## The Sky Dart

![AMC Sky Dart utility/logistics spacecraft](/assets/images/demo/skydart.svg)
*The Sky Dart*

### Specifications

Height
: Approximately 9.5 m

Width Overall
: 8.8 m

Mass
: 2500 kg (empty)

Fuel and Oxidizer Mass
: 2500 kg

MTOW
: 6250 kg

Maximum Landing Acceleration
: 18 $\frac m {s^2}$ (empty) 7.2 $\frac m {s^2}$ (at MTOW)

Maximum Landing Speed
: 4.2 $\frac m s$ (empty) 2.6 $\frac m s$ (at MTOW)

Minimum Main Engine Thrust
: 2.0 kN

Maximum Main Engine Thrust
: 20.0 kN

> **Maximum landing specifications assume simultaneous touchdown of all landing feet, and zero lateral or rotational velocity.**

## Overview

The Sky Dart is a physically accurate simulation of a *sensible* fictionalized spacecraft. Although it has a throttle control and a joystick, it does not handle like a helicopter, and it definitely does not handle like an airplane!

### Throttle

The throttle control is a large T-handle control on the left side of the cockpit that operates the main engine. The engine is at the bottom of the spacecraft and exhausts downward. The thrust from the engine is directed upwards. Some simple rules to remember are:
* When the thrust is equal to the weight of the ship, it will begin to hover. 
* If the thrust is greater than the weight, the ship will begin to accelerate upwards. 
* If the thrust is less than the weight and the ship is aloft, it will begin to accelerate downwards.

> **As you operate the rocket engine, fuel is consumed and the weight of the ship decreases. Hovering under manual control requires constant vigilance.**

![Sky Dart hovering with equal and opposite thrust and weight](/assets/images/demo/skydart_hover.svg)
*Sky Dart hovers (or maintains constant acceleration) with equal and opposite thrust and weight*

### Joystick

Using only the throttle, you can go up (ascend) or down (descend), but there is no way to control your sideways motion. For this, use the joystick. Moving the joystick does not *directly* move the ship sideways. Instead, it operates small rockets (called *attitude control thrusters*) on the side of the ship that make the ship rotate. For example, if you push the stick forward, it will make the ship rotate (or *pitch*) forward.

![Sky Dart pitching forward using attitude control thrusters](/assets/images/demo/skydart_pitchforward.svg)
*Sky Dart pitches forward using attitude control thrusters*

When the ship is leaning forward, the main engine thrust and the weight are not balanced. Some of the thrust force is directed in the forward direction. A physicist would say that *the thrust vector now has a forward component*. The forward part of the thrust, though small, will make the ship accelerate in the forward direction. Its forward speed increases.

![Sky Dart moving forward after pitching forward](/assets/images/demo/skydart_moveforward.svg)
*Sky Dart accelerates forward because its thrust direction is partly forward*

Because the ship is leaning, the *vertical component* of the main engine thrust isn't as large as it used to be. If the ship was hovering before, it will begin to accelerate downward at the same time that it accelerates forward. Because of this, you have to increase the main thrust slightly to hold your hovering altitude while accelerating forward.

> **Once your ship has the pitch or roll angle you want, you can let the joystick return to its centered position. The ship will automatically hold its pitch or roll angle until you change it.**

### Getting From Point A to Point B

All of these ideas come together when you try to fly from one place to another, and land safely:

![Sky Dart moving from point A to point B](/assets/images/demo/skydart_pointatob.svg)

### Basic Instruments

While you are flying, you can judge your altitude, orientation, and velocity by looking out the window, but you will do better if you use the instruments in the cockpit. The radar panel shows your height above the ground (ALT) in meters, vertical speed (VSPD) and horizontal speed (HSPD) in meters/second.

The "cross pointer" display also shows your horizontal speed as a sideways (left to right) and forward (and backward) component using the two orange needles. 

![radar panel](/assets/images/demo/radarpanel.png){: width="150" }

When you are in mountainous terrain, or at night, it's hard to tell exactly how much your ship is tipped, relative to the horizon. Use the *artificial horizon* display to judge your pitch or banking angle.

![imu and artificial horizon panel](/assets/images/demo/imu_panel.png){: width="150" }

### How to Yaw or Spin Left or Right

With the joystick you can tip the ship forward or backward, and left or right, and any combination of those. Whatever direction you tip the ship, it will begin to accelerate in that direction. But neither of those motions lets you turn the ship to face a different direction. The left or right-ward spinning motion is called *yaw*. The joystick does not have a yaw function, but if you press the **ALT CTRL** button in front of you, then joystick left-right movement will give you left-right yawing motion. Press **ALT CTRL** again to return to the normal joystick movement.

> **Yawing the ship does not by itself change its direction of motion. If your ship is moving forwards, and you yaw 90 degrees to the left, the ship will continue moving in its original direction. From your point of view, the ship will now be moving to the right!**