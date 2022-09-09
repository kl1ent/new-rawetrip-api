# ⚙ Tab system

### Simple tab system

{% hint style="info" %}
To do something like this, you can refer to the [ui.md](../variables/ui.md "mention")
{% endhint %}

```lua
--> Main table
local example = {}

--> Combobox with tab names
local tabs = ui.add_combobox("tabs", { "first", "second", "third" })

--> Elements in first tab
example.first_tab.checkbox = ui.add_checkbox("Checkbox")
example.first_tab.slider = ui.add_sliderint("Slider")

--> Elements in second tab
example.second_tab.combobox = ui.add_combobox("Combo", { "1", "2", "3" })
example.second_tab.button = ui.add_button("Button")

cheat.push_callback("on_paint", function()
    --> Parsing first tab
    for key, val in pairs(example.first_tab) do
        val:set_visible(tabs:get() == 0 and true or false)
    end

    --> Parsing second tab
    for key, val in pairs(example.second_tab) do
        val:set_visible(tabs:get() == 1 and true or false)
    end
end)
```
