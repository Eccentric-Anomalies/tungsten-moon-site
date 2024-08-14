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
Hover mode commands the joystick and throttle to zero out any *acceleration* of the ship, while maintaining the current vertical and horizontal *rates* or *speed*. The vertical speed is shown in the **VS** seven-segment display on the autopilot panel, while the horizontal speeds are shown the two green diamond "bugs" on the cross-pointer display:

![AMC Sky Dart autopilot cross-pointer horizontal speed bugs](/assets/images/demo/hspd_stablerate.png){: width="150" }

### Typical Transition from HOVR OFF to HOVR ON
The following diagram shows how the ship's dynamic state changes when HOVR mode is engaged.

![AMC Sky Dart autopilot HOVR MODE ON](/assets/images/demo/skydart_hovrmode.svg)

Engaging HOVR mode *captures* the current vertical and horizontal speeds of the ship, then tries to maintain them. Once engaged, you can change the captured speeds using the round vernier throttle knob and the joystick.

### Changing Vertical Speed While HOVR MODE is Engaged
While HOVR MODE is ON, use the vernier throttle to adjust the vertical speed. If you adjust the vertical speed to be ZERO, then the autopilot will also capture the altitude above terrain, and will continue to make adjustments to hold the captured altitude.

The following graphic shows an example of using HOVR mode to slow descent and hold a true hover at 308 m above the surface.

![AMC Sky Dart autopilot HOVR MODE slowing descent](/assets/images/demo/skydart_hovrzerorate.svg)

## HSPD (Horizontal Speed) MODE
Engaging HOVR mode automatically engages HSPD mode and captures your current horizontal speed. When HSPD is engaged, disengage it again by pressing the **HSPD MODE** button; HOVR mode will not be affected. Regardless of the HSPD mode, disengaging HOVR will force HSPD OFF. In other words, HSPD requires the vertical speed to be controlled by autopilot at all times.

While HSPD mode is ON, the joystick moves the horizontal speed setpoint, shown by the position of the two green diamond speed bugs on the cross-pointer display. If PROP CTRL is OFF, then the position of the joystick corresponds to the rate at which the speed bugs move. If you release the joystick, the setpoint stays where it is. If you push the joystick fully forward, the forward speed setpoint will increase at a constant rate. If you release the joystick again, the setpoint will freeze at its current position.

The following graphic shows an example of using HSPD mode to slow the horizontal speed from 8 $\frac m s$ to 4 $\frac m s$:

![AMC Sky Dart autopilot HSPD MODE changing forward speed](/assets/images/demo/skydart_hspdchange.svg)

## X10
Turning X10 on when HSPD mode is on increases the joystick sensitivity by a factor of 10. In [PROP CTRL](#prop-ctrl-proportional-control) mode, it changes the full scale joystick deflection from 1 $\frac m s$ to 10 $\frac m s$.

## PROP CTRL (Proportional Control)
Proportional control mode changes how the joystick moves the horizontal speed setpoint bugs on the cross-pointer display. With PROP CTRL engaged, the setpoint bug position will track the joystick position. If the joystick is released, then the setpoint speeds will both be zero. Toggling PROP CTRL ON, then OFF is a good way to quickly reset the speed setpoints to zero.

When PROP CTRL and X10 are both active, full deflection of the joystick will command a horizontal speed of 10 $\frac m s$. If X10 is off, then the maximum horizontal speed you can set is 1 $\frac m s$.

### Landing With PROP CTRL
One of the best uses of PROP CTRL is during the final approach to a landing pad. The final approach should be at a low (1-2 $\frac m s$) vertical and horizontal speed. Once the ship is over the center of the pad, engage PROP CTRL to arrest all forward motion; the ship will then descend straight down until contacting the pad or terrain.