# Extended Communication Ranges - ExComm
This mod aim to add a menu to engage a conversation with NPC outside the regular comm range by adding a Long Range Comm Beam to your ship.

## What it does ?
This mod grants your ship the ability to use the "Long Range Comm Beam" (LRCB), which instead of granting you an instant communication with anybody within 40km grants you the ability to reach ships and stations in your current sector with an accurate precision after a little delay.
It open a menu when using Long Range Scan Mode with a selected eligible target (outside of the Map Menu) to engage conversation. But, there is some limitations (see below).

## How to use it ?
*First and foremost, you must know that your ship technical limitation won't grant you the ability to focus the LRCB to reach a target in another sector.*
*You must also know that the LRCB is only able to work on a entity (ship or station) you're able to target, otherwise, it can't be precise enough to be engaged (target must be visible, either on radar, satellite or in close proximity one of your station, and in the same sector).*
*And last but not least, to activate the LRCB, you must be piloting your ship, for the same reason that you can't active the Long Range Scan Mode if you're not piloting.*
*It should be obvious, but it need to be remembered.*
- First, target a ship or station (by clicking it on your screen, radar, or pressing "T" (default binding) after selecting it on you map).
- ~~Next, outside the Map (if you opened it), right click on the ship or station (on your screen, or screen edge if you're not facing it, or on the radar) and click the action "Extended Comm".~~
- In this "NoSirNukes" version, you need to activate you Long Range Scan Mode. A menu will appear to ask you if you want to by-pass the Long Range Scan power to your Long Range Comm Beam in order to contact the target.
- While the LRCB is calibrating to your target, your HUD may flicker a bit because of the powersurge, you may also here the "Long Range Scan Mode" activation sound since the LRCB is reliying on it (that's why the power surge).
- The LRCB have a "Time To Calibrate" (TTC), you will be notified in the notification area how many time it will take depending of the distance between ou and your target, please note that the minimum charging time is 2 seconds.
- Wait a few seconds and TADA, your communication with the target ship is established

**TLDR; Target someone, activate your Long Range Scan Mode**

## Technically ?
- Listen to activity.scan_longrange
- add_player_choice when a target is selected, waiting for input
- Add a little sound + hud effect for 2 seconds while the "Long Range Comm Beam" is calibrating/focusing
- Calculate the time of charge depending of the target distance to your ship (ratio is Distance(m) / 300000 in seconds), but can't be lower than 2 seconds
- Engage convo with target pilot
- Reset HUD

## Requirements ?
- NONE

## Redistribution and modification

### BSD 2-Clause License

#### Copyright (c) 2026, laryakan

You are free to use, modify and redistribute any code or assets of mine which is not directly extracted from the game as soon as you mention the above Copyright.
A link to my github is provided below. A little mention is all I ask.

- github : https://github.com/laryakan/excomm
- nexus : https://www.nexusmods.com/x4foundations/mods/1698
- nexus user : https://next.nexusmods.com/profile/Laryakan
