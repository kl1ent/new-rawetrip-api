# 🚶♂ entity

## Functions:

### get\_local

`entity.get_local():` <mark style="color:purple;">`entity`</mark>

### get\_player\_by\_index

`entity.get_player_by_index(player_index: number):` <mark style="color:purple;">`entity`</mark>

| Name              | Type         | Description   |
| ----------------- | ------------ | ------------- |
| **player\_index** | **`number`** | player\_index |

### get\_weapon\_by\_player

`entity.get_player_by_index(player: entity):` <mark style="color:purple;">`weapon`</mark>

| Name       | Type         | Description |
| ---------- | ------------ | ----------- |
| **player** | **`entity`** | player      |

### get\_players

`entity.get_player_by_index(ignore_team: boolean):` <mark style="color:purple;">`table`</mark>

| Name             | Type          | Description  |
| ---------------- | ------------- | ------------ |
| **ignore\_team** | **`boolean`** | ignore\_team |

## Classes:

### :get\_name

`<entity>:get_name():` <mark style="color:purple;">`string`</mark>

### :get\_weapons

`<entity>:get_weapons(index: number):` <mark style="color:purple;">`weapon`</mark>

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **index** | **`number`** | index       |

### :get\_index

`<entity>:get_index():` <mark style="color:purple;">`number`</mark>

### :get\_dormant

`<entity>:get_dormant():` <mark style="color:purple;">`boolean`</mark>

### :get\_team

`<entity>:get_team():` <mark style="color:purple;">`number`</mark>

### :is\_alive

`<entity>:is_alive():` <mark style="color:purple;">`boolean`</mark>

### :get\_velocity

`<entity>:get_velocity():` <mark style="color:purple;">`vector`</mark>

### :get\_absorigin

`<entity>:get_absorigin():` <mark style="color:purple;">`vector`</mark>

### :get\_angles

`<entity>:get_angles():` <mark style="color:purple;">`vector`</mark>

### :get\_player\_hitbox\_pos

`<entity>:get_player_hitbox_pos():` <mark style="color:purple;">`vector`</mark>

### :get\_muzzle\_pos

`<entity>:get_muzzle_pos():` <mark style="color:purple;">`vector`</mark>

### :get\_player\_bone\_pos

`<entity>:get_player_bone_pos():` <mark style="color:purple;">`vector`</mark>

### :get\_shoot\_pos

`<entity>:get_shoot_pos():` <mark style="color:purple;">`vector`</mark>

### :has\_heavy\_arm

`<entity>:has_heavy_arm():` <mark style="color:purple;">`vector`</mark>

### :is\_scoped

`<entity>:is_scoped():` <mark style="color:purple;">`vector`</mark>

### :get\_health

`<entity>:get_health():` <mark style="color:purple;">`vector`</mark>

### :get\_bbox

`<entity>:get_bbox():` <mark style="color:purple;">`vector`</mark>

### :get\_body\_yaw

`<entity>:get_body_yaw():` <mark style="color:purple;">`number`</mark>

### :m\_flposeparameter

`<entity>:m_flposeparameter()[index: number]`

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **index** | **`number`** | -           |

```lua
cheat.push_callback("on_frame_net", function(stage)
    if (stage == enum_frames.frame_start) then
        local player = entity.get_local()
        
        if (player == nil or not player:is_alive()) then
            return
        end
        
        local flags = player:get_prop_int("CBasePlayer", "m_fFlags")
        local on_ground = bit.band(flags, 1) == 1
        
        if (not on_ground) then
            player:m_flposeparameter()[7] = 1 --> Static legs
        end
    end
end)
```

### :set\_render\_pose

`<entity>:set_render_pose(index: number, value: number)`

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **index** | **`number`** | index       |
| **value** | **`number`** | value       |

### :draw\_hitbox

`<entity>:draw_hitbox(hitbox: number, col: color, duration: number, ignore_z: boolean)`

| Name          | Type          | Description |
| ------------- | ------------- | ----------- |
| **hitbox**    | **`number`**  | hitbox      |
| **col**       | **`color`**   | col         |
| **duration**  | **`number`**  | duration    |
| **ignore\_z** | **`boolean`** | ignore\_z   |

### :set\_model\_index

`<entity>:set_model_index(index: number)`

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **index** | **`number`** | index       |

### :get\_model

`<entity>:get_model():` <mark style="color:purple;">`model`</mark>

### :get\_prop\_int / :get\_prop\_float / :get\_prop\_bool / :get\_prop\_string

`<entity>:get_prop_int():` <mark style="color:purple;">`number`</mark> <mark style="color:purple;"></mark><mark style="color:purple;"></mark>&#x20;

`<entity>:get_prop_float():` <mark style="color:purple;">`number`</mark> <mark style="color:purple;"></mark><mark style="color:purple;"></mark>&#x20;

`<entity>:get_prop_bool():` <mark style="color:purple;">`boolean`</mark> <mark style="color:purple;"></mark><mark style="color:purple;"></mark>&#x20;

`<entity>:get_prop_string():` <mark style="color:purple;">`string`</mark>

### :set\_prop\_int / :set\_prop\_float / :set\_prop\_bool / :set\_prop\_string

`<entity>:set_prop_int(var: number)`

`<entity>:set_prop_float(var: number)`

`<entity>:set_prop_bool(var: boolean)`

`<entity>:set_prop_string(var: string)`
