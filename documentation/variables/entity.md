# 🚶♂ entity

## Functions:

### get_local

`entity.get_local():` `entity`

### get_player_by_index

`entity.get_player_by_index(player_index: number):` `entity`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **player_index** | **`Number`** | player_index   |

### get_weapon_by_player

`entity.get_player_by_index(player: entity):` `weapon`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **player** | **`Entity`** | player   |

### get_players

`entity.get_player_by_index(ignore_team: boolean):` `table: entity, ...`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **ignore_team** | **`Boolean`** | ignore_team   |

## Classes:

### :get_name()

`<entity>:get_name():` `string`

### :get_weapons()

`<entity>:get_weapons(index: number):` `weapon`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **index** | **`Number`** | index   |

### :get_index()

`<entity>:get_index():` `number`

### :get_dormant()

`<entity>:get_dormant():` `boolean`

### :get_team()

`<entity>:get_team():` `number`

### :is_alive()

`<entity>:is_alive():` `boolean`

### :get_velocity()

`<entity>:get_velocity():` `vector`

### :get_absorigin()

`<entity>:get_absorigin():` `vector`

### :get_angles()

`<entity>:get_angles():` `vector`

### :get_player_hitbox_pos()

`<entity>:get_player_hitbox_pos():` `vector`

### :get_muzzle_pos()

`<entity>:get_muzzle_pos():` `vector`

### :get_player_bone_pos()

`<entity>:get_player_bone_pos():` `vector`

### :get_shoot_pos()

`<entity>:get_shoot_pos():` `vector`

### :has_heavy_arm()

`<entity>:has_heavy_arm():` `vector`

### :is_scoped()

`<entity>:is_scoped():` `vector`

### :get_health()

`<entity>:get_health():` `vector`

### :get_bbox()

`<entity>:get_bbox():` `vector`

### :get_body_yaw()

`<entity>:get_body_yaw():` `number`

### :m_flposeparameter()

`<entity>:m_flposeparameter()[ number ]:` `number`

### :set_render_pose()

`<entity>:set_render_pose(index: number, value: number):`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **index** | **`Number`** | index   |
| **value** | **`Number`** | value   |

### :draw_hitbox()

`<entity>:draw_hitbox(hitbox: number, col: color, duration: number, ignore_z: boolean):`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **hitbox** | **`Number`** | hitbox   |
| **col** | **`Color`** | col   |
| **duration** | **`Number`** | duration   |
| **ignore_z** | **`Boolean`** | ignore_z   |

### :set_model_index()

`<entity>:set_model_index(index: number):`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **index** | **`Number`** | index   |

### :get_model()

`<entity>:get_model():` `model`

### :get_prop_int() / :get_prop_float() / :get_prop_bool() / :get_prop_string()

`<entity>:get_prop_int():` `number`
`<entity>:get_prop_float():` `number`
`<entity>:get_prop_bool():` `boolean`
`<entity>:get_prop_string():` `string`

### :set_prop_int() / :set_prop_float() / :set_prop_bool() / :set_prop_string()

`<entity>:set_prop_int(var: number):`
`<entity>:set_prop_float(var: number):`
`<entity>:set_prop_bool(var: boolean):`
`<entity>:set_prop_string(var: string):`
