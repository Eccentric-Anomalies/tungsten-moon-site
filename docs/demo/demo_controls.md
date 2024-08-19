---
layout: default
title: Sky Dart Controls
parent: Tungsten Moon Demo
nav_order: 5
---

# Sky Dart Controls
You can fly the Sky Dart with a keyboard and mouse, using an optional game controller (e.g. XBOX), with PC flight simulator joysticks (e.g. HOTAS), or with an OpenXR-compatible VR headset and hand-controllers. 

All of the Sky Dart user inputs (i.e. buttons, joysticks, etc.) are controllable in the cockpit using either your computer mouse, or your virtual VR fingers or hands. A subset of these inputs may be mapped or assigned to a game controller, joystick, or computer keyboard. Following are the default assignments for these inputs; you may customize them using a control panel in the Sky Dart cockpit.

{: .no_toc }


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>
 
## Default Keyboard Map
![AMC Sky Dart default keyboard map](/assets/images/demo/keyboard-map.svg)

{: .note }
The SHIFT key toggles the ALT CTRL button in the cockpit:

### ALT CTRL Mode
ALT CTRL mode changes the behavior of some inputs:

|  | ALT CTRL ON | ALT CTRL OFF |
|:--:|:--:|:--:|
| **CAMERA INPUTS** | pans L-R and U-D  | moves L-R and F-B  |
| **JOYSTICK INPUTS** | left-right is YAW | left-right is ROLL |

## Default Game Controller Map (and Steam Deck)
Tungsten Moon supports many video game controllers in a generic way:

### XBOX
![AMC Sky Dart XBOX controller map](/assets/images/demo/controller-map.svg)

### PlayStation
![AMC Sky Dart PS controller map](/assets/images/demo/controller-ps-map.svg)

### Steam Deck
![AMC Sky Dart Steam Deck controller map](/assets/images/demo/controller-steamdeck-map.svg)

## Default VR Controller Inputs
The default map should work for most OpenXR-compatible VR hand controllers.

![AMC Sky Dart Steam Deck controller map](/assets/images/demo/vr-controller-map.svg)

{: .note }
The default VR controller input assignments may not be modified.

## Default Mouse Inputs
If you are not using a VR headset, you can:
* Use the mouse LEFT button to press buttons in the cockpit.
* Hover the mouse cursor over the throttle, vernier throttle, or joystick, and hold the LEFT button move the control.
* Hover the mouse cursor over the throttle and use the mouse scroll wheel to change the throttle setting.
* Use the mouse RIGHT button to move the camera view direction.


{: .note }
The default mouse input assignments may not be modified.

## Steam Deck Mouse Emulation
By default, tapping the Steam Deck touchscreen with your fingertip will emulate the mouse LEFT button press. Move your viewpoint using the camera movement buttons (blue) on the controller, then tap your finger to press the virtual cockpit buttons on the screen. You can also use your finger directly on the screen to move the throttle, vernier throttle, and joystick.

The Steam Deck is very customizable. For example, you can configure the trackpad to emulate a mouse with the RIGHT mouse button held down for very responsive camera view panning.

## Configuring PC Flight Sim Hardware
If you are using a conventional PC joystick (typically used with flight simulators) with a throttle control, use the input mapping panel (in the cockpit) to map the **THR A+** and **THR A-** to the throttle's full and cut positions, respectively.

We recommend assigning **THR +** and **THR -** to a pair of buttons or an up/down toggle on your PC joystick. This input is important for controlling the vernier throttle AND sets the vertical ascent or descent rate when you are in autopilot hover mode.

{: .note }
The **THR MAX**, **THR MIN**, **THR +**, and **THR -** inputs should **NOT** be mapped to a PC throttle lever. 

## Reassigning Control Inputs

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