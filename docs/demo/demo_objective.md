---
layout: default
title: Object of the Game
parent: Tungsten Moon Demo
nav_order: 3
---

## Object of the Game
What is the object of the game?

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