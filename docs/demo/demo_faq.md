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

### I can not start game. It brings me back to steam page (crashes without explanation).
This is common if the computer system and/or GPU are not powerful enough to run Tungsten Moon, or if the game files are corrupted. If you are confident your system is powerful enough, then we recommend [verifying the integrity of the game files](https://help.steampowered.com/en/faqs/view/0C48-FCBD-DA71-93EB) in Steam. If this does not help, we would like to work with you to figure out what is happening. Please contact us at: [support@eccentricanomalies.com](mailto:support@eccentricanomalies.com)

### There is no explanation of what I am doing. No menu. No settings. What is the point of the game?
Tungsten Moon is first and foremost a spaceflight simulator. Not the Star Wars sort of simulator, with guns and controls that make it act like an airplane. The first point of the game is to figure out how to fly the ship. There are guides on Steam and at the website (https://tungstenmoon.com), but the Sky Dart is pretty simple and you can control everything with just a mouse.

### I figured out how to fly the Sky Dart. What next?
Congratulations! Flying the Sky Dart is pretty hard. The next thing you can learn to do is fly the Sky Dart over greater distances and even into orbit. There are 20 landing pads scattered across the moon and a panel on the Sky Dart that keeps track of how many you have landed on. Can you find them all? The final game will have more complicated goals to complete in order to progress and survive, but for the Demo we've kept it pretty simple.

### When I push the throttle forward not much happens, but eventually I start going up, instead of forward. How do I go forward?
Like all *real* lunar and planetary landers, your main engine points *down*, so your reaction acceleration is *up*. Use the joystick on the right to tip the spacecraft in the direction you want to go, then apply the throttle to move in that direction. There are also some pretty nifty autopilot modes that can help.

### When I use the throttle to move forward, I wound up about 10 km in the sky and never came down. That can't be right, can it? Is gravity only at the surface?
Gravity follows an inverse-square law. If you fly 30 km above the surface of the moon, which has a 300 km radius, the gravity is only reduced by 19%. Unless you have launched yourself into orbit, or an escape trajectory, you probably will come down again. Pro-tip: for local flying, avoid getting above 2 km altitude. Judicious use of the throttle is called for.

### The instructions say that the ALT CTRL button will make the joystick left-right movement produce a "yawing" movement. What is yaw?
[Yawing movement in an airplane](https://howthingsfly.si.edu/flight-dynamics/roll-pitch-and-yaw) or boat is what a rudder does. It is rotation around a (local to the spaceship) vertical axis.

### What kind of spaceship am I in? Is this like a Star Wars spaceship?
The Tungsten Moon Sky Dart is similar to the [Apollo Lunar Module](https://en.wikipedia.org/wiki/Apollo_Lunar_Module). There is big rocket that points down, controlled by the throttle, and a bunch of smaller rockets around the outside that make the ship tip or spin by using the joystick. It is a little bit like a helicopter, but without the aerodynamic response.

### How high do I have to go to get into orbit?
Since there is no air on the Tungsten Moon, there is no need to get high at all. You can enter orbit at any altitude, as long as you fly fast enough and parallel to the surface of the moon. If you are below 5 km or so, you do run the risk of colliding with mountains, however. Once you reach orbit you can turn off your engine and coast around the moon indefinitely. Each orbit takes about 45 minutes. It's pretty.

### Every time I go to land, I end up starting over. What happened?
You landed too fast, crashed and died. Your speed at landing should generally be at or below 1 m/s vertically *and* horizontally or you run the risk of ripping your landing gear off (this kills the pilot).

### How do I know if my computer will run Tungsten Moon?
Most gaming computers with 4 GB of dedicated video RAM and a discrete (plug in card) graphics processor (GPU) made by Nvidia or AMD will be fine. To be sure, install the free Tungsten Moon Demo and see how it works. Press Ctrl-Shift-H (in that order) to display the FPS on the screen. A FPS of 60 or better is excellent. We do not recommend playing Tungsten Moon if your frame rate is consistently lower than 60 FPS.

### Should I use Steam to download and play Tungsten Moon Demo?
Although the demo will always be available on from the [Tungsten Moon Demo releases Github page](https://github.com/Eccentric-Anomalies/Tungsten-Moon-Demo-Releases/releases), we recommend [Steam](https://store.steampowered.com/app/3104900/Tungsten_Moon/) for its easy access to beta versions and its automatic version updating. If you play using a VR headset, then Steam offers a seamless experience for selecting between the VR and non-VR versions of the game.

### How do I use my OpenXR headset (e.g. Quest 3) with Tungsten Moon Demo?
We recommend running Tungsten Moon Demo from Steam. Configure your headset as an OpenXR device and use SteamVR (free) on the Steam platform. Launch Tungsten Moon Demo from your library and select the VR option from the popup menu.

### Am I limited to flying to or from the landing pads in Tungsten Moon?
Some landing pads are spawn points for the game, but you are free to fly anywhere on the surface of the moon.

### I am trying to find a pad? Where is the light?
The landing pad lights are only visible when you are closer than 10 km to it any direction. Note: if your altitude is above 10 km, you will not see it! 

### I keep flying toward pads but I don't ever find them. I set the heading correctly.
Since the Sky Dart is a realistic spacecraft and not an airplane, the heading shown on the artificial horizon is not automatically the direction you are traveling! When setting a heading, also check there is no horizontal drift shown on the cross-pointer gauge to the right. The heading must be correct and the horizontal drift must be centered (check with the x1 range to be sure!). This must be monitored both when starting a trip and before the lander passes an altitude of 2 km. The radar and cross-pointer do not operate above 2 km since there is no return from the radar above that altitude.

### Can the Sky Dart spaceship enter orbit around the Tungsten Moon?
Yes! The Sky Dart spacecraft, when fully fueled, is capable of reaching a stable orbit around the moon, with enough remaining fuel to leave orbit and safely land on the surface again. Please note, however, that this is quite difficult to do without running out of fuel! The orbital period is about 45 minutes.

### Ok. So how DO I put the Sky Dart into orbit?
Orbital velocity near the surface of the moon is approximately 700 m/s. The goal is to reach that speed, while flying near the surface (between 5-10 km altitude), with no vertical velocity. As you increase your speed and approach 700 m/s, watch the periapsis and apoapsis values (on the IMU panel) carefully. Kill your thrust the moment you achieve orbit, as it's very easy to enter a hyperbolic escape trajectory by accident. An ideal, approximately circular orbit is achieved when both values are in the range of 5-10. To do this, you need to accelerate with the Sky Dart at a very steep angle, almost horizontal to the surface. Monitor your altitude on the IMU or radar carefully, to avoid ascending too high or too quickly, and to avoid crashing on the surface.

### Why do I run out of fuel when flying long distances? You said I could go anywhere!
If you are flying long distances by moving sideways while hovering (for example, by using “hover mode”), then you are not making the most efficient use of your propulsion system. The most efficient way of flying *anywhere* on the moon is to use maximum thrust to launch into either a parabolic trajectory (shorter trips) or orbit (longer distances). While orbital flight can literally take you anywhere on the surface, the Sky Dart in Tungsten Moon Demo is not equipped with navigation equipment needed to pinpoint a specific landing site.

You can plan parabolic flights with fair accuracy by using this physics projectile distance formula:

$v \approx 40 \sqrt{D}$
{: style="text-align: center;"}

*v*
: Speed in m/s

*D*
: Horizontal distance to fly, in km

Launch at an angle of about 30 degrees from vertical, at full thrust, while adjusting your pitch to maintain HVEL and VVEL as close to each other as possible. When you reach the desired velocity (*v* in the equation above), cut your thrust and note your speed. On the other end, as you are descending, cut in full thrust when your speed reaches the speed you noted on the way up.

{: .note}
Since the distance formula assumes an *instantaneous* launch at the speed, *v*, this formula will tend to overshoot the desired distance because the Sky Dart will take some time to reach the velocity, at which point it will already be at a high altitude and down range. Practice with short hops to get a feel for how much you should decrease the launch velocity to hit your destination.

Hover mode works well with short flights (a few km) and speeds below 100 m/s. If you are flying above rough terrain, your top speed will be considerably lower because the autopilot can’t reliably maintain altitude over rough terrain. For greater distances, you can manage your own hover and accelerate to much higher horizontal speeds. Use the basic distance formula and the chronometer to estimate your arrival time at your destination:

$t = \frac {1000 \cdot D} v$
{: style="text-align: center;"}

*v*
: HVEL speed in m/s

*D*
: Horizontal distance to fly, in km

*t*
: Time needed for the trip, in seconds

Establish a constant HVEL as soon as possible, then compute the time of flight and add it to the current chronometer time to estimate your arrival time. As the appointed time draws near, keep a sharp eye out for the approaching landing site and be prepared to decelerate and land.
