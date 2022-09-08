# 📞 Callbacks list

## How to use game events:

{% embed url="https://wiki.alliedmods.net/Counter-Strike:_Global_Offensive_Events" %}
Official CS:GO events
{% endembed %}

```lua
cheat.push_callback("on_event", function(event)
    if (event:get_name() == "player_hurt") then
        --- code
    end
end)
```

## How to use callbacks:

### on\_paint

```lua
cheat.push_callback("on_paint", function()
    render.rect_filled(200, 200, 100, 20, color(255, 255, 255, 255))
end)
```

### on\_createmove

```lua
cheat.push_callback("on_createmove", function(cmd)
    cmd.viewangles.z = 50
end)
```

### after\_prediction

```lua
cheat.push_callback("after_prediction", function(cmd)
    cmd.viewangles.z = 50
end)
```

| Name                | Type         | Description              |
| ------------------- | ------------ | ------------------------ |
| **forwardmove**     | **`number`** | Forward / backward speed |
| **sidemove**        | **`number`** | Left / right speed       |
| **upmove**          | **`number`** | Up / down speed          |
| **viewangles**      | **`vector`** | Player view angles       |
| **buttons**         | **`number`** | Player buttons           |
| **command\_number** | **`number`** | Current command number   |

### on\_frame\_net

{% hint style="info" %}
Stages - [enum\_frames.md](../enumerations/enum\_frames.md "mention")
{% endhint %}

```lua
cheat.push_callback("on_frame_net", function(stage)
    if (stage == enum_frames.frame_start) then
        cheat.notify("frame_start")
    end
end)
```

### on\_override\_view

```lua
cheat.push_callback("on_override_view", function(view)
    view.fov = 20
end)
```

| Name               | Type         | Description |
| ------------------ | ------------ | ----------- |
| **fov**            | **`number`** | -           |
| **angles**         | **`vector`** | -           |
| **origin**         | **`vector`** | -           |
| **height**         | **`number`** | -           |
| **height\_old**    | **`number`** | -           |
| **width**          | **`number`** | -           |
| **width\_old**     | **`number`** | -           |
| **viewmodel\_fov** | **`number`** | -           |
| **x**              | **`number`** | -           |
| **x\_old**         | **`number`** | -           |
| **y**              | **`number`** | -           |
| **y\_old**         | **`number`** | -           |

### on\_unload

```lua
cheat.push_callback("on_unload", function()
    cheat.notify("Script unloaded!")
end)
```

### on\_shot

```lua
cheat.push_callback("on_shot", function(shot_info)
    cheat.notify(shot_info.target_name)
end)
```

| Name               | Type         | Description                                |
| ------------------ | ------------ | ------------------------------------------ |
| **target\_name**   | **`string`** | Target name                                |
| **result**         | **`string`** | Shot result                                |
| **client\_hitbox** | **`string`** | Hitbox                                     |
| **server\_hitbox** | **`string`** | Hitbox                                     |
| **client\_damage** | **`number`** | Actual shot damage                         |
| **server\_damage** | **`number`** | Actual shot damage                         |
| **hitchance**      | **`number`** | Actual shot hit chance                     |
| **backtrack**      | **`number`** | Amount of ticks the player was backtracked |
| aim\_point         | **`string`** | Actual shot aim point                      |
