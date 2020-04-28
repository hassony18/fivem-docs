---
title: respawnPlayerPedEvent
weight: 551
---

Called when a player respawns.

Parameters
----------

```
string player, table content
```

- **player**: The player that has spawned.
- **content**: A table contains the information about player's respawn point.

Examples
--------
This example prints the name of the player and the reason why the player has disconnected to the server console.
##### Lua Example:
```lua
-- source is global here, don't add to function
AddEventHandler("respawnPlayerPedEvent", function(player, content)
	print(GetPlayerName(player).." has spawned at "..tostring(content.posX)..", "..tostring(content.posY)..", "..tostring(content.posZ))
end)
```
