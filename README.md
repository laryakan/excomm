# Extended Comm
This mod aim to add an interact button to engage a conversation with NPC outside the regular comm range.

## What it does ?
This mod grants your ship the ability to use the "Long Range Comm Beam" (LRCB), which instead of granting you an instant communication with anybody within 40km grants you the ability to reach ships in your current sector with an accurate precision after a little delay.
It simply add an interact button on eligible target (outside of the Map Menu) to engage conversation. It's limited to the current sector since you can't interact with target outside this range.

## How to use it ?
*First and foremost, you must know that your ship technical limitation wont grant you the ability to focus the LRCB to reach a target in another sector.*
*You must also know that the LRCB can only be focused on a target you can see on your radar (including ships detected with a satellite or close to a allied station).*
*And last but not least, to activate the LRCB, you must be piloting your ship.*
*It should be obvious, but it need to be remembered.*
- First, target a ship (by clicking it on your screen, radar, or pressing "T" (default binding) after selecting it on you map)
- Next, outside the Map if you opened it, right click on the ship (on your screen, or screen edge if you're not facing it or on the radar) and click the action "Extended Comm"
- While the LRCB is calibrating to you target, you HUD may flicker a bit because of the powersurge, you may also here the "Long Range Scan Mode" sound since the LRCB is reliying on it
- Wait a few seconds and TADA, your communication with the target ship is established
- You will be notify or the progress of the calibration in your notification area (lower left or HUD)

**TLDR; Right click on a ship, select "Extended Comm"**

## Will the LRCB will get an update ?
Maybe. Since station aren't moving in space, our team may do something to contact station managers in the future.

## Technically ?
- Listen to md.Interact_Menu_API.Get_Actions
- md.Interact_Menu_API.Add_Action on class.destructible + ship when player is piloting
- Add a little sound + hud effect for 2 seconds while the "Long Range Comm Beam" is calibrating/focusing
- Engage convo with target pilot

## Requirements ?
- SirNukes Mod Support APIs

- github : https://github.com/laryakan/excomm
- nexus : https://www.nexusmods.com/x4foundations/mods/<tba>
- nexus user : https://next.nexusmods.com/profile/Laryakan
