# Extended Comm
This mod aim to add an interact button to engage a conversation with NPC outside the regular comm range.

## What it does ?
It simply add an interact button on eligible target (outside of the MapMenu) to engage conversation. It's limite to the current sector since you can't interact with target outside this range.

## Technically ?
- Listen to md.Interact_Menu_API.Get_Actions
- md.Interact_Menu_API.Add_Action on class.destructible + ship when player is piloting
- Add a little sound + hud effect for 2 seconds while the "Long Range Comm Beam" is charging
- Engage convo with target pilot

## Requirements ?
- SirNukes Mod Support APIs

- github : https://github.com/laryakan/excomm
- nexus : https://www.nexusmods.com/x4foundations/mods/<tba>
- nexus user : https://next.nexusmods.com/profile/Laryakan
