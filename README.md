# Titans Productions Dirt System

> `EXPORTS`

**Get dirt level data value:**

`exports.tp_dirtsystem:GetDirtLevel()`

**Get dirt level (Percentage):**

`exports.tp_dirtsystem:GetFixedDirtLevel()`

**Add dirt level:**

`exports.tp_dirtsystem:AddPlayerDirtLevel(value)`

**Set dirt level:**

`exports.tp_dirtsystem:SetPlayerDirtLevel(value)`

**Clear (reset) player dirt level to clean:**

`exports.tp_dirtsystem:ClearPlayerDirtLevel()`

**Update dirt level (save in server):**

`exports.tp_dirtsystem:UpdatePlayerDirtLevel()`


**Check if the player dirt level data have been loaded: **

`exports.tp_dirtsystem:IsPlayerLoaded()`

> `EVENTS`

To update the temperature, `"tp_dirtsystem:GetTemperature"` (Client Event) must be called with `temperature value` as the first and only required parameter, for example: 

This event must be called when using another temperature script and not our own temperature system.

**Update temperature from another script:**

```lua
TriggerEvent("tp_dirtsystem:GetTemperature", temp) -- Client Side
```
