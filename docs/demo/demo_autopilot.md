---
layout: default
title: Sky Dart Autopilot Modes
parent: Tungsten Moon Demo
nav_order: 4
usemathjax: true
---

# Sky Dart Autopilot Modes
For the sophisticated space pilot.

{: .no_toc }


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

## The Autopilot Control Panel
Like many small aircraft, the Sky Dart has a basic autopilot control panel just below the pilot's primary window.

![AMC Sky Dart autopilot control panel](/assets/images/demo/autopilot_panel.png)
*The Sky Dart autopilot control panel*

### Autopilot Functions In A Nutshell

| Autopilot Mode | When Activated | When Deactivated |
|:--:|:--:|:--:|
| RATE MODE | joystick commands a rotation **rate**  | joystick commands a rotation **acceleration** and deactivates HOVR MODE  |
| HOVR MODE | ship holds current **vertical rate** *and* activates HSPD MODE  | deactivates HSPD MODE |
| HSPD MODE | ship holds current **horizontal rates** and deactivates PROP CTRL | deactivates PROP CTRL |
| X10 | HSPD joystick inputs are $\pm$ 10 $\frac m s$ or $\frac m {s^2}$| HSPD joystick inputs are $\pm$ 1 $\frac m s$ or $\frac m {s^2}$ | 
| PROP CTRL | joystick: horizontal rates in $\frac m s$| joystick: **change** in horizontal rates in $\frac m {s^2}$ | 

The following sections cover each mode in more detail.

## RATE MODE
When the Sky Dart is powered up, the autopilot has RATE MODE active by default. With RATE MODE off, the joystick directly operates the attitude control thrusters. The ship is very difficult to control RATE MODE off, and the only time it should be deactivated is if there is a fault in the autopilot.

### RATE MODE ON
![AMC Sky Dart autopilot RATE MODE ON](/assets/images/demo/skydart_ratemode.svg)

{: .note }
With RATE MODE ON, any rotational motion of the ship can be stopped simply by letting go of the joystick.

### RATE MODE OFF
![AMC Sky Dart autopilot RATE MODE ON](/assets/images/demo/skydart_noratemode.svg)


## HOVR (Hover) MODE
Hover mode commands the joystick and throttle to zero out any *acceleration* of the ship, while maintaining the current vertical and horizontal *rates* or *speed*. The vertical speed is shown in the **VS** seven-segment display on the autopilot panel, while the horizontal speeds are shown the two green diamond indicators on the cross-pointer display:

![AMC Sky Dart autopilot cross-pointer horizontal velocity diamonds](/assets/images/demo/hspd_stablerate.png){: width="150" }

### Typical Transition from HOVR OFF to HOVR ON
The following diagram shows how the ship's dynamic state changes when HOVR mode is engaged.
![AMC Sky Dart autopilot HOVR MODE ON](/assets/images/demo/skydart_hovrmode.svg)

Engaging HOVR mode *captures* the current vertical and horizontal velocity of the ship, then tries to maintain it. Once engaged, you can change the captured velocities using the round vernier throttle knob and the joystick.

### Changing Vertical Speed While HOVR MODE is Engaged
While HOVR MODE is ON, use the Vernier Throttle to adjust the vertical speed. If you adjust the vertical speed to be ZERO, then the autopilot will also capture the altitude above terrain, and will continue to make adjustments to hold the captured altitude.

## HSPD (Horizontal Speed) MODE

## PROP CTRL (Proportional Control)