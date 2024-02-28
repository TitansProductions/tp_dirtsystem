# Titans Productions Dirt System

> `EXPORTS`

**Get Dirt Level:**

`exports.tp_dirtsystem:GetDirtLevel()`

**Update Dirt Level Based on the type (increasing / decreasing). Types are located in the configuration file.**

`exports.tp_dirtsystem:UpdateDirtLevelBasedOnType(type)`

Those exports must be called in your river, bath or any script that you want to increase or decrease dirt progress.

> `EVENTS`

**Get Current Dirt Level:**

```lua
AddEventHandler("tp_dirtsystem:getCurrentDirtLevel", function(dirtLevel)
    -- your action
end)
```

To update the temperature, `"tp_dirtsystem:GetTemperature"` (Client Event) must be called with `temperature value` as the first and only required parameter, for example: 

This event must be called when using another temperature script and not our own temperature system.

**Update temperature from another script:**

```lua
TriggerEvent("tp_dirtsystem:GetTemperature", temp)
```
