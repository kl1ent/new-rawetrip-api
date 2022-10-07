# 🔫 weapon

## Functions:

{% hint style="info" %}
Access functions listed below via [<mark style="color:purple;">get\_weapon\_by\_player</mark>](entity.md#get\_weapon\_by\_player) <mark style="color:purple;"></mark> function
{% endhint %}

### :is\_empty

`<weapon>:is_empty():` <mark style="color:purple;">`boolean`</mark>

### :can\_fire

`<weapon>:can_fire():` <mark style="color:purple;">`boolean`</mark>

### :is\_non\_aim

`<weapon>:is_non_aim():` <mark style="color:purple;">`boolean`</mark>

### :can\_double\_tap

`<weapon>:can_double_tap():` <mark style="color:purple;">`boolean`</mark>

### :get\_name

`<weapon>:get_name():` <mark style="color:purple;">`string`</mark>

### :get\_icon

`<weapon>:get_icon():` <mark style="color:purple;">`string`</mark>

```lua
--> Example
local weapon_font = render.setup_weapon_font(12)

cheat.push_callback("on_paint", function()
    local player = entity.get_local()

    if (player == nil) then
        return
    end

    local player_weapon = entity.get_weapon_by_player(player)

    if (player_weapon == nil) then
        return
    end

    local weapon_icon = player_weapon:get_icon()

    render.text(weapon_font, 200, 200, color(255, 255, 255, 255), weapon_icon)
end)
```

### :get\_spread

`<weapon>:get_spread():` <mark style="color:purple;">`number`</mark>

### :get\_inaccuracy

`<weapon>:get_inaccuracy():` <mark style="color:purple;">`number`</mark>
