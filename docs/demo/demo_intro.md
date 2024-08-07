---
layout: default
title: Tungsten Moon Demo
nav_order: 2
has_children: true
---
# Tungsten Moon: The Demo (V0.1.8)

The Tungsten Moon Demo includes the basic flight mechanics of the full Tungsten Moon game, with a minimal set of exploration goals.

{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>



## Controls
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

### Respawn Points
The right-hand side of the cockpit has a small panel that you can use to view the available spawn points in the game. A valid spawn point is any **base** landing pad, with an identifier of the form `Pad n:0`, that you have already visited. When you play the game for the first time, Pads 0:0, 1:0, 2:0, 3:0, AND 4:0 in the "visited" state by default, and can be used as spawn points.

In future versions of the game, some base pads will *not* be preset as "visited" and you will need to find them and visit them *yourself* before you can use them as spawn points.

The spawn panel includes the following controls and displays:
* Use the button labeled "NEXT BASE" to scroll through the list of available base pads.
* The selected base pad is shown on a seven-segment display as `bb:nn`, where `bb` is the base group identifier (currently the values range from 0 to 4), and `nn` is the individual pad within the group (the base is always 0).
* The number of pads in this base group that you have safely landed on is shown next.
* The number of pads available for landing in the base group is shown last.
* Use the button on the right, labeled "GOTO BASE" to immediately respawn at the selected base pad.

Respawning resets the day/time clock to the day and time when the game was last (automatically) saved. With each session playing the game, the clock will continue to advance from the last save. This means that you will see each spawn point go through the full day/night cycle over a period of ten hours of playing time. With multiple days, you will also see the phases of the planet in the sky change as the Tungsten Moon orbits around it. You could even witness an eclipse of the sun, though the event is rare.

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

---

## How to Get Started
* Run the program.
* Allow the spacecraft to settle onto the surface, or immediately press PG-UP to begin accelerating away from the surface.
* Once off the ground, press SHIFT (ALTERNATE control mode toggle), then hold left-arrow or right-arrow to start rotating your craft. This will enable you to view the planet and/or sun in the sky (if present).
* Press SHIFT (toggle back out of ALTERNATE control mode)l, then use the right stick (controller) or the arrow keys to pitch/roll into a sideways attitude so you can accelerate horizontally. If you can bring your horizontal speed up to 700 m/s you will enter orbit. Try to adjust A ALT. and P ALT. values to be between 3 and 10 km. Watch the moon roll by.. 
* Try lifting off, then landing softly back on the surface.
* Try lifting off, then moving horizontally a few hundred meters, then landing softly on the surface with has little horizontal motion as possible.

Check the [Tungsten Moon YouTube channel](https://www.youtube.com/channel/UCCZ3MdbmQ5ZqAspNrOZUuTw) for examples and more tips.

---

## Current Features
* The custom sky shader includes a rotating field of 10,000 random stars, a sun, and a planet. All of these are in motion, relative to each other, at speeds and scales that are physically reasonable. This means that although they *appear* to be stationary, they are actually in full motion.
* Star field brightness is automatically adjusted between barely visible and brilliant, depending on whether the sun or planet are visible in the sky.
* The motion simulation accounts for the tungsten moon itself spinning on its axis. The current rotation period is ten hours. This should give rise to Coriolis effects if you know where to look, although this has not been carefully verified yet.
* The input scheme supports not only keyboard and mouse, but also the Xbox, Playstation and Steam Deck controllers. All control keys have been assigned to make the experience of moving between keyboard and controller more intuitive. There is no user re-configuration possible yet.
* The executable file currently works with the Valve Steam Deck, using the latest Proton emulation layer. The performance is excellent, though it runs hot.
* There are five starting locations on the moon that you can choose from, with a very primitive UI. Each starting location consists of a set of four landing pads for a total of twenty in the game. Each pad has an identifier and location label, and directions and distance to several other pads.
* Landing pads have a red flashing beacon that turns green once you have landed safely on them. Can you find and land on all twenty pads?
* A "radar altimeter" mode activates below 2000 meters altitude and will read correctly down to the surface of the planet.
* Velocity is reported as ground-relative horizontal and vertical components.
* An attitude "nav ball" helps to orient the pilot.
* A horizontal drift indicator shows the cockpit-relative forward/backwards and left/right motion of the ship. This is derived from doppler radar data and will only operate below the 2000 meter radar altitude limit, and when the ship is within 45 degrees of horizontal. Three speed ranges, 1x, 10x, and 100x are selectable with buttons on the display.
* To help with achieving orbit, apoapsis and periapsis altitudes are reported ("ORBITAL APSIDES" AA and PA, respectively) for the current spacecraft altitude and velocity vector.

---
