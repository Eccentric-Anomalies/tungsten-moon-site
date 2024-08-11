---
layout: default
title: Sky Dart Controls
parent: Tungsten Moon Demo
nav_order: 4
---

## Sky Dart Controls
Some inputs perform an alternate function. Pressing the right shoulder button on the controller or the SHIFT key on the keyboard toggles the ALTERNATE control mode. There is also an in-cockpit UI button that you can activate with a mouse or VR controller.

---

### Interior View
* D-Pad (controller) or WASD (keyboard) control the view direction inside the cockpit. By toggling the ALTERNATE control, you can use these inputs to move your viewpoint forward/backward and left/right.
* If you are using a mouse, hold the RMB (right mouse button) and move the mouse to pan your view. Note: the Steam Deck can be configured with the trackpad emulating a mouse with the RMB held down.

---

### Flight Controls
* The right stick (controller) or direction keys (keyboard) control pitch and roll thrusters. 
* The right left/right (controller) or left/right keys (keyboard) activate the yaw (rotate left/right) thrusters in ALTERNATE mode.
* The left stick x-axis (VR controller) controls the yaw thrusters. (V0.1.6)
* Keyboards that have a numeric keypad also work in the Orbiter style: pitch control with 8/2, roll with 4/6, and yaw with 1/3.

---

### Main Thrust Control
* The in-cockpit THROTTLE handle works with a mouse or VR hand controller. With a XBOX/PS game controller, the left trigger controls the THROTTLE.
* On a game controller, the left trigger is used to manually control the thrust from zero to maximum. This is useful for quick adjustments as you approach a landing.
* The VERNIER throttle lever is just to the right of the main THROTTLE control. Use this to make small, precise adjustments to the throttle setting. You can grab this with a mouse or VR hand controller. The VR/XBOX/PS game controller LEFT stick vertical axis, or keyboard Ctrl + PG-UP or Ctrl + PG-DN, or the keypad Ctrl+ or Ctrl- directly controls the vernier. To remap this input, select the THR + and THR - inputs on the UI mapping panel. (V0.1.6)
* On a keyboard, PG-UP and PG-DN (keypad + or -) immediately set and hold full or zero thrust.
* To configure an analog flightsim throttle, use the input mapping panel to map the THR A+ and THR A- to the throttle control's full and cut positions, respectively.
* The effect of your throttle input is displayed on the IMU accelerometer. The nominal gravitational acceleration on the surface of the moon is 1.6 m/s/s. If you hold the ship acceleration at 1.6 during flight, then you  will be assured of maintaining a constant velocity, relative to the surface (which could include *no* velocity). When the ship is flown at an angle, it will accelerate sideways under thrust, and slightly *more* than 1.6 m/s/s acceleration is required to maintain altitude.

---

### Other Controls
* Menu button or Q or ESC key will quit the program.
* X button or X key will toggle attitude rate mode (ON by default).
* Y button or Y key will toggle vertical speed mode (VSPEED). In this mode, the vernier throttle control adjusts the desired ascent/descent rate in m/s. (V0.1.6)
* The ALARM button will light if there is any system failure, or the autopilot VSPEED mode is disengaged involuntarily. Press the ALARM to extinguish the button and silence any audible alarms. (V0.1.6)
* There is an in-cockpit landing light toggle switch. There is no controller button or keyboard key mapped to this switch.
* There is an in-cockpit button for refilling the propellant tank. There is no controller button or key for this. You can only refill the tank when you have landed on an official, round landing pad.
* B controller button or R key or LEFT VR controller B/Y button will restart at your current scenario location.
* Left stick PUSH (controller) or V key or LEFT VR controller A/X button will reset your view position.
* There is an in-cockpit button to reset the attitude indicator. When the ship is stationary on the ground, the internal gyroscope and accelerometers can determine the rotation axis of the moon, and the ship's orientation with respect to the horizon; pressing reset will initialize the indicator to show true heading (0 degrees N, 90 degrees E, etc.) and tilt. When the ship is aloft, and **not** rotating, then the reset button will force the indicator to show heading of zero degrees and level horizon, regardless of the ship's actual position. This is because there are no external references (i.e. gps satellites or ground beacons) that can determine true orientation or position. Future versions of the game will probably incorporate additional navigational aids and attitude indicator modes.
* The horizontal drift indicator has three ranges (1x, 10x, and 100x) selectable with "radio buttons". They correspond to +/-1, +/-10, and +/-100 m/s speed, full scale.