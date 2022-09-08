# ⚙ UI Interaction

### Example of ui interaction

{% hint style="info" %}
To do something like this, you can refer to the [ui.md](../variables/ui.md "mention")
{% endhint %}

```lua
--> New checkbox
local checkbox = ui.add_checkbox("Checkbox")

--> New slider
local slider = ui.add_sliderint("Slider")

--> New combo
local combo = ui.add_combobox("Combo", { "First", "Second", "Third" })

--> New hotkey
local hotkey = ui.add_hotkey("Hotkey")

cheat.push_callback("on_paint", function()

    --> Checkbox interaction
    local checkbox_boolean = checkbox:get() --> Returns boolean [ true / false ]
    checkbox:set(true) --> Sets boolean [ true / false ]
    checkbox:set_visible(false) --> Sets visible [ true / false ] - def: [true]

    --> SliderInt interaction
    local slider_number = slider:get() --> Returns number
    slider:set(15) --> Sets number
    slider:set_visible(false) --> Sets visible [ true / false ] - def: [true]

    --> Combo interaction
    local combo_number = combo:get() --> Returns number
    local combo_items = combo:get_items() --> Returns items: { , ... }
    combo:set(1) --> Sets select
    combo:set_visible(false) --> Sets visible [ true / false ] - def: [true]
    combo:set_items({ "1", "2", "3", "4", "5" }) --> Sets items

    --> Hotkey interaction
    local hotkey_boolean = hotkey:get() --> Returns boolean [ true / false ]
    local hotkey_mode = hotkey:get_mode() --> Returns number
    hotkey:set_visible(false) --> Sets visible [ true / false ] - def: [true]

end)
```
