# Extended Comm
This mod aim to add an interact button to engage a conversation with NPC outside the regular comm range by adding a Long Range Comm Beam to your ship.

## What it does ?
This mod grants your ship the ability to use the "Long Range Comm Beam" (LRCB), which instead of granting you an instant communication with anybody within 40km grants you the ability to reach ships in your current sector with an accurate precision after a little delay.
It simply add an interact button on eligible target (outside of the Map Menu) to engage conversation. But, there is some limitations (see below).

## How to use it ?
*First and foremost, you must know that your ship technical limitation won't grant you the ability to focus the LRCB to reach a target in another sector.*
*You must also know that the LRCB is only able to work on a entity (ship) you're able to target, otherwise, it can't be precise enough to be engaged (target must be visible, either on radar, satellite or in close proximity one of your station, and in the same sector).*
*And last but not least, to activate the LRCB, you must be piloting your ship, for the same reason that you can't active the Long Range Scan Mode if you're not piloting.*
*It should be obvious, but it need to be remembered.*
- First, target a ship (by clicking it on your screen, radar, or pressing "T" (default binding) after selecting it on you map).
- Next, outside the Map (if you opened it), right click on the ship (on your screen, or screen edge if you're not facing it, or on the radar) and click the action "Extended Comm".
- While the LRCB is calibrating to your target, your HUD may flicker a bit because of the powersurge, you may also here the "Long Range Scan Mode" activation sound since the LRCB is reliying on it (that's why the power surge).
- The LRCB have a "Time To Calibrate" (TTC), you will be notified in the notification area how many time it will take depending of the distance between ou and your target, please note that the minimum charging time is 2 seconds.
- Wait a few seconds and TADA, your communication with the target ship is established

**TLDR; Right click on a ship (outside the map), select "Extended Comm" then wait things to happen**

**Warning ! HUD flashes may (or may not) cause an epileptic seizure, I made an alternate version with a lower calibration frequency to prevent this**

## Will the LRCB will get an update ?
Maybe. The actual version of the LRCB know where a ship cockpit is to focus on it, but station are too large and with too many different configurations for the LRCB to target the specific room where a manager is.
This may change in the future.

## Technically ?
- Listen to md.Interact_Menu_API.Get_Actions
- md.Interact_Menu_API.Add_Action on class.destructible + ship when player is piloting
- Add a little sound + hud effect for 2 seconds while the "Long Range Comm Beam" is calibrating/focusing
- Calculate the time of charge depending of the target distance to your ship (ratio is Distance(m) / 100000 in seconds), but can't be lower than 2 seconds
- Engage convo with target pilot
- Reset HUD

## Requirements ?
- SirNukes Mod Support APIs

- github : https://github.com/laryakan/excomm
- nexus : https://www.nexusmods.com/x4foundations/mods/1698
- nexus user : https://next.nexusmods.com/profile/Laryakan
