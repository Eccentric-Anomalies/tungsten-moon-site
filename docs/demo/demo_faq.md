---
layout: default
title: Frequently Asked Questions (FAQ)
parent: Tungsten Moon Demo
nav_order: 6
usemathjax: true
---

## Frequently Asked Questions

{: .no_toc }


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

### How do I know if my computer will run Tungsten Moon?
Most gaming computers with 4 GB of dedicated video RAM and a discrete (plug in card) graphics processor (GPU) made by Nvidia or AMD will be fine. To be sure, install the free Tungsten Moon Demo and see how it works. Press Ctrl-Shift-H (in that order) to display the FPS on the screen. A FPS of 60 or better is excellent. We do not recommend playing Tungsten Moon if your frame rate is consistently lower than 60 FPS.

### Should I use Steam to download and play Tungsten Moon Demo?
Although the demo will always be available on from the [Tungsten Moon Demo releases Github page](https://github.com/Eccentric-Anomalies/Tungsten-Moon-Demo-Releases/releases), we recommend [Steam](https://store.steampowered.com/app/3104900/Tungsten_Moon/) for its easy access to beta versions and its automatic version updating. If you play using a VR headset, then Steam offers a seamless experience for selecting between the VR and non-VR versions of the game.

### How do I use my OpenXR headset (e.g. Quest 3) with Tungsten Moon Demo?
We recommend running Tungsten Moon Demo from Steam. Configure your headset as an OpenXR device and use SteamVR (free) on the Steam platform. Launch Tungsten Moon Demo from your library and select the VR option from the popup menu.

### Am I limited to flying to or from the landing pads in Tungsten Moon?
Some landing pads are spawn points for the game, but you are free to fly anywhere on the surface of the moon.

### I am trying to find a pad? Where is the light?
The landing pad lights are only visible when you are closer than 10 km from it in any axis. Note: if your altitude is above 10 km, you will not see it! 

### I keep flying toward pads but I don't ever find them. I set the heading correctly.
Since the Sky Dart is a realistic spacecraft and not an airplane, the heading shown on the artificial horizon is not automatically the direction you are traveling! When setting a heading, also check there is no horizontal drift shown on the cross-pointer gauge to the right. The heading must be correct and the horizontal drift must be centered (check with the x1 range to be sure!). This must be monitored both when starting a trip and before the lander passes an altitude of 2 km. The radar and cross-pointer do not operate above 2 km since there is no return from the radar above that altitude.

### Can the Sky Dart spaceship enter orbit around the Tungsten Moon?
Yes! The Sky Dart spacecraft, when fully fueled, is capable of reaching a stable orbit around the moon, with enough remaining fuel to leave orbit and safely land on the surface again. Please note, however, that this is quite difficult to do without running out of fuel! The orbital period is about 45 minutes.

### Ok. So how DO I put the Sky Dart into orbit?
Orbital velocity near the surface of the moon is approximately 700 m/s. The goal is to reach that speed, while flying near the surface (between 5-10 km altitude), with no vertical velocity. As you increase your speed and approach 700 m/s, watch the periapsis and apoapsis values (on the IMU panel) carefully. Kill your thrust the moment you achieve orbit, as it's very easy to enter a hyperbolic escape trajectory by accident. An ideal, approximately circular orbit is achieved when both values are in the range of 5-10. To do this, you need to accelerate with the Sky Dart at a very steep angle, almost horizontal to the surface. Monitor your altitude on the IMU or radar carefully, to avoid ascending too high or too quickly, and to avoid crashing on the surface.

### Why do I run out of fuel when flying long distances? You said I could go anywhere!
If you are flying long distances by moving sideways while hovering (for example, by using “hover mode”), then you are not making the most efficient use of your propulsion system. The most efficient way of flying *anywhere* on the moon is to use maximum thrust to launch into either a parabolic trajectory (shorter trips) or orbit (longer distances). While orbital flight can literally take you anywhere on the surface, the Sky Dart in Tungsten Moon Demo is not equipped with navigation equipment needed to pinpoint a specific landing site.

You can plan parabolic flights with fair accuracy by using this physics trajectory distance formula:

$$\\
v \approx 40 \sqrt{D}
\\$$

*v*:
Speed in m/s

*D*:
Horizontal distance to fly, in km

Launch at an angle of about 30 degrees from vertical, at full thrust, while adjusting your pitch to maintain HVEL and VVEL as close to each other as possible. When you reach the desired velocity (*v* in the equation above), cut your thrust and note your speed. On the other end, as you are descending, cut in full thrust when your speed reaches the speed you noted on the way up.

{: .note}
Since the distance formula assumes an *instantaneous* launch at the speed, *v*, this formula will tend to overshoot the desired distance because the Sky Dart will take some time to reach the velocity, at which point it will already be at a high altitude and down range. Practice with short hops to get a feel for how much you should decrease the launch velocity to hit your destination.

Hover mode works well with short flights (a few km) and speeds below 100 m/s. If you are flying above rough terrain, your top speed will be considerably lower because the autopilot can’t reliably maintain altitude over rough terrain. For greater distances, you can manage your own hover and accelerate to much higher horizontal speeds. Use the basic distance formula and the chronometer to estimate your arrival time at your destination:

$$\\
t = \frac {1000 \cdot D} v
\\$$

*v*:
HVEL speed in m/s

*D*:
Horizontal distance to fly, in km

*t*:
Time needed for the trip, in seconds

Establish a constant HVEL as soon as possible, then compute the time of flight and add it to the current chronometer time to estimate your arrival time. As the appointed time draws near, keep a sharp eye out for the approaching landing site and be prepared to decelerate and land.
