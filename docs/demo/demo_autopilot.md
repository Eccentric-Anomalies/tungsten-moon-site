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

### Functions In A Nutshell

| Autopilot Mode | When Activated | When Deactivated |
|:--:|:--:|:--:|
| RATE MODE | joystick commands a rotation **rate**  | joystick commands a rotation **acceleration** and deactivates HOVR MODE  |
| HOVR MODE | ship holds current **vertical rate** *and* activates HSPD MODE  | deactivates HSPD MODE |
| HSPD MODE | ship holds current **horizontal rates** and deactivates PROP CTRL | deactivates PROP CTRL |
| PROP CTRL | joystick commands horizontal rates | joystick commands **change** in horizontal rates | 

The following sections cover each mode in more detail.

## RATE MODE
By default, when the Sky Dart is powered up, the autopilot is has RATE MODE active. With RATE MODE off, the joystick directly operates the attitude control thrusters. The ship is very difficult to control RATE MODE off, and the only time it should be deactivated is if there is a fault in the autopilot.

### RATE MODE ON
![AMC Sky Dart autopilot RATE MODE ON](/assets/images/demo/skydart_ratemode.svg)

{: .note }
With RATE MODE ON, any rotational motion of the ship can be stopped simply by letting go of the joystick.

### RATE MODE OFF
![AMC Sky Dart autopilot RATE MODE ON](/assets/images/demo/skydart_noratemode.svg)


## HOVR (Hover) MODE

## HSPD (Horizontal Speed) MODE

## PROP CTRL (Proportional Control)