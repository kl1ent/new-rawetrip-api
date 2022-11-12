# 👀 esp

## Functions:

### push\_flag

`esp.push_flag(name: string, color: color, func: function)`

| Name      | Type           | Description                                                        |
| --------- | -------------- | ------------------------------------------------------------------ |
| **name**  | **`string`**   | Flag text                                                          |
| **color** | **`color`**    | Flag color                                                         |
| **func**  | **`function`** | Function that will be called for each entity while drawing the ESP |

```lua
esp.push_flag("Flag name", color(255, 255, 255, 255), function(player)
    cheat.notify(player:get_name())

    --- [true] - so that the flag is displayed
    --- [false] - so that the flag is not displayed
    return true
end)
```
