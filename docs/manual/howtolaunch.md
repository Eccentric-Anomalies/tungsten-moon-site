---
layout: default
title: How to Run Tungsten Moon Demo
parent: Tungsten Moon Manual
nav_order: 1
---

# How to Download and Run Tungsten Moon Demo

{: .no_toc }


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

## Run Tungsten Moon Demo in Steam (Easy)

If you don't already have a Steam account, visit the [Steam website](https://store.steampowered.com/about/) and download their free app for Windows or Linux. It doesn't cost anything to create a Steam account and you can download and run all the free games or demos in the Steam store.

Using your Steam account, search for Tungsten Moon in the Steam store, or visit the [Tungsten Moon store page](https://store.steampowered.com/app/3104900/Tungsten_Moon/) in your browser. There you can install and download the free Tungsten Moon Demo game.

### Steam Deck

Tungsten Moon Demo may be installed on your Steam Deck (Valve's hand-held gaming platform). Valve has not formally given Tungsten Moon a compatibility rating with Steam Deck, but we routinely use it as part of our development and testing process. Although the desktop version of Tungsten Moon uses a keyboard and/or mouse for some functionality, you can use the D-Pad view controls and the touchscreen to activate any in-cockpit UI elements using the Steam Deck, just as you would if you were using a mouse on desktop, or your virtual finger in VR.

## Download Executables from Github (Almost Easy)

The Tungsten Moon Demo is always available from [Github](https://github.com/Eccentric-Anomalies/Tungsten-Moon-Demo-Releases/releases). Download the binary executable that matches your operating system and choice of VR vs. desktop:

|             |      Windows       |         Linux         |
| :---------: | :----------------: | :-------------------: |
| **Desktop** |  TungstenMoon.exe  |  tungstenmoon.x86_64  |
|  **VR/XR**  | TungstenMoonXR.exe | tungstenmoonxr.x86_64 |

If you are using one of these binaries to play Tungsten Moon in VR, we recommend using Steam VR as the OpenXR runtime. This is what we use for testing.

## Running the Game

After a loading screen, Tungsten Moon immediately places you in the cockpit of a Sky Dart lunar logistics spacecraft, which you can begin flying right away. You can pause and/or bring up a game panel (menu) by pressing the [ESC] key, controller menu button or left VR controller B/Y button while in the game:

![game menu panel](/assets/images/manual/game_menu_panel.png){: width="800" }

The panel has two modes: GAME and INPUTS. Use the [INPUTS mode to change the default keyboard or game controller inputs](https://tungstenmoon.com/docs/manual/controls.html#reassigning-control-inputs).

## Game Saves

Tungsten Moon automatically saves your game only when your spacecraft lands safely at a pad or site where fuel and consumables are available. This guarantees that you will never find yourself stuck in a location where you can't reload fuel and continue the game.

There is no other mechanism for saving your Tungsten Moon game.

## GAME Panel

Use the GAME panel to pause/unpause, reload, start a new game, or quit to desktop:

### CONTINUE FLIGHT

While you the GAME panel is active, the game is paused. Press CONTINUE FLIGHT to resume from where you left off.

### RELOAD FROM LAST SAFE FUEL STOP

Your Sky Dart spacecraft can be resupplied only from certain landing pads or zones in the game. When you land safely at one of these your game is automatically saved. Press this button to reload your game from the point of your *last safe* landing at a location with fuel. This option guarantees that you will always be able to get out of a tough spot by returning to the last location where you were able to fully resupply your Sky Dart with consumables. 


### ERASE SAVED GAME - START NEW

Tungsten Moon does not allow multiple saved games at the same time. Use this option to end your current game and start a new one from the beginning.

{: .note }
If you are writing Forth software to replace or add to the default firmware in the cockpit flight computer, you must choose the ERASE SAVED GAME option in order for your new software to be loaded. This is because the RAM image of data and code in your cockpit computer is included in the saved game; the firmware cannot be updated without performing a cold reboot, which only should be done at the start of a new game.

### QUIT TO DESKTOP

Choose this option to exit Tungsten Moon. Any progress you have made since your *last safe landing* will be lost.

{: .note }
All of the options on this manual except CONTINUE FLIGHT require confirmation with the PROCEED button. Press CANCEL if you change your mind.