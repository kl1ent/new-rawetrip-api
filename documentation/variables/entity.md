# 🚶♂ entity

## Functions:

### get\_local

`entity.get_local():` <mark style="color:purple;">`entity`</mark>

Returns a pointer to the local player.

### get\_player\_by\_index

`entity.get_player_by_index(player_index: number):` <mark style="color:purple;">`entity`</mark>

| Name              | Type         | Description   |
| ----------------- | ------------ | ------------- |
| **player\_index** | **`number`** | player\_index |

Returns a pointer to the specified player.

### get\_weapon\_by\_player

`entity.get_weapon_by_index(player: entity):` <mark style="color:purple;">`weapon`</mark>

| Name       | Type         | Description |
| ---------- | ------------ | ----------- |
| **player** | **`entity`** | player      |

Returns a pointer to the player's weapon entity.

### get\_players

`entity.get_players(ignore_team: boolean):` <mark style="color:purple;">`table`</mark>

| Name             | Type          | Description  |
| ---------------- | ------------- | ------------ |
| **ignore\_team** | **`boolean`** | ignore\_team |

Returns the table of pointers to entities.

## Classes:

### :get\_animstate

`<entity>:get_animstate():` <mark style="color:purple;">`table`</mark>

<details>

<summary>Field</summary>

m\_flUpVelocity \
m\_bInHitGroundAnimation \
m\_bOnGround \
m\_fDuckAmount \
m\_fLandingDuckAdditiveSomething \
m\_flCurrentFeetYaw \
m\_flCurrentTorsoYaw \
m\_flEyeYaw \
m\_flFeetCycle \
m\_flFeetSpeedForwardsOrSideWays \
m\_flFeetSpeedUnknownForwardOrSideways \
m\_flFeetYawRate \
m\_flGoalFeetYaw \
m\_flHeadHeightOrOffsetFromHittingGroundAnimation m\_flLastClientSideAnimationUpdateTime \
m\_flLastOriginZ \
m\_flLeanAmount \
m\_flMovingFraction \
m\_flPitch \
m\_flSpeedNormalized \
m\_flStopToFullRunningFraction \
m\_flTimeSinceStartedMoving \
m\_flTimeSinceStoppedMoving \
m\_iLastClientSideAnimationUpdateFramecount\
m\_velocity \
m\_vLastOrigin \
m\_vOrigin \
m\_vVelocityX \
m\_vVelocityY

### :max\_desync\_delta

`<anim_state>:max_desync_delta():` <mark style="color:purple;">`number`</mark>

</details>

Returns the player animstate.

### :get\_animlayer

`<entity>:get_animlayer(index: number):` <mark style="color:purple;">`table`</mark>

| Name      | Type         | Description     |
| --------- | ------------ | --------------- |
| **index** | **`number`** | Animlayer index |

<details>

<summary>Field</summary>

m\_bClientBlend \
m\_flBlendIn \
m\_flCycle \
m\_flPlaybackRate \
m\_flPrevCycle \
m\_flWeight \
m\_flWeightDeltaRate \
m\_nDispatchSequence \
m\_nOrder \
m\_nSequence

</details>

Returns the player animlayer.

### :get\_sequence\_activity

`<entity>:get_sequence_activity(sequence: number):` <mark style="color:purple;">`number`</mark>

| Name         | Type         | Description |
| ------------ | ------------ | ----------- |
| **sequence** | **`number`** | Sequence    |

Returns the player sequence activity.

### :get\_name

`<entity>:get_name():` <mark style="color:purple;">`string`</mark>

Returns the player name.

### :get\_weapons

`<entity>:get_weapons(index: number):` <mark style="color:purple;">`weapon`</mark>

Returns a table containing pointers to every weapon entity the player is currently carrying.

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **index** | **`number`** | index       |

### :get\_index

`<entity>:get_index():` <mark style="color:purple;">`number`</mark>

Returns the index of the player.

### :get\_dormant

`<entity>:get_dormant():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the player is dormant.

### :get\_team

`<entity>:get_team():` <mark style="color:purple;">`number`</mark>

Returns the player team number.

### :is\_alive

`<entity>:is_alive():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the player is alive.

### :get\_velocity

`<entity>:get_velocity():` <mark style="color:purple;">`vector`</mark>

Returns the velocity vector of the player.

### :get\_absorigin

`<entity>:get_absorigin():` <mark style="color:purple;">`vector`</mark>

Returns the absolute position vector of the player.

### :get\_angles

`<entity>:get_angles():` <mark style="color:purple;">`vector`</mark>

Returns the angles of the player.

### :get\_player\_hitbox\_pos

`<entity>:get_player_hitbox_pos():` <mark style="color:purple;">`vector`</mark>

Returns the position of the specified hitbox.

### :get\_muzzle\_pos

`<entity>:get_muzzle_pos():` <mark style="color:purple;">`vector`</mark>

Returns the position of the muzzle.

### :get\_player\_bone\_pos

`<entity>:get_player_bone_pos():` <mark style="color:purple;">`vector`</mark>

Returns the position of the specified bone.

### :get\_shoot\_pos

`<entity>:get_shoot_pos():` <mark style="color:purple;">`vector`</mark>

Returns the position of the shoot.

### :has\_heavy\_arm

`<entity>:has_heavy_arm():` <mark style="color:purple;">`vector`</mark>

Returns <mark style="color:green;">`true`</mark>, if the player has heavy armor

### :is\_scoped

`<entity>:is_scoped():` <mark style="color:purple;">`vector`</mark>

Returns <mark style="color:green;">`true`</mark>, if the player is scoped.

### :get\_health

`<entity>:get_health():` <mark style="color:purple;">`vector`</mark>

Returns the player health.

### :get\_bbox

`<entity>:get_bbox():` <mark style="color:purple;">`table`</mark>

Returns a table containing <mark style="color:blue;">`x`</mark>, <mark style="color:blue;">`y`</mark>, <mark style="color:blue;">`w`</mark>, and <mark style="color:blue;">`h`</mark> values.

### :get\_body\_yaw

`<entity>:get_body_yaw():` <mark style="color:purple;">`number`</mark>

Returns the player body yaw.

### :m\_flposeparameter

`<entity>:m_flposeparameter()[index: number]:` <mark style="color:purple;">`number`</mark>

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **index** | **`number`** | -           |

Returns the player pose parameters.

### :set\_render\_pose

`<entity>:set_render_pose(index: number, value: number)`

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **index** | **`number`** | index       |
| **value** | **`number`** | value       |

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
            player:set_render_pose(6, 1) --> Static legs
        end
    end
end)
```

Sets the values of the pose parameters.

### :draw\_hitbox

`<entity>:draw_hitbox(hitbox: number, col: color, duration: number, ignore_z: boolean)`

| Name          | Type          | Description |
| ------------- | ------------- | ----------- |
| **hitbox**    | **`number`**  | hitbox      |
| **col**       | **`color`**   | col         |
| **duration**  | **`number`**  | duration    |
| **ignore\_z** | **`boolean`** | ignore\_z   |

Draws a specific player hitbox.

### :set\_model\_index

`<entity>:set_model_index(index: number)`

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **index** | **`number`** | index       |

Sets the index of the model to the player.

### :get\_model

`<entity>:get_model():` <mark style="color:purple;">`model`</mark>

Returns the player model.

## Getting prop values

{% tabs %}
{% tab title="int" %}
`<entity>:get_prop_int(class_name: string, prop_name: string):` <mark style="color:purple;">`number`</mark>

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
{% endtab %}

{% tab title="float" %}
`<entity>:get_prop_float(class_name: string, prop_name: string):` <mark style="color:purple;">`number`</mark>

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
{% endtab %}

{% tab title="bool" %}
`<entity>:get_prop_bool(class_name: string, prop_name: string):` <mark style="color:purple;">`boolean`</mark>

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
{% endtab %}

{% tab title="string" %}
`<entity>:get_prop_string(class_name: string, prop_name: string):` <mark style="color:purple;">`string`</mark>

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
{% endtab %}

{% tab title="entity" %}
`<entity>:get_prop_entity(class_name: string, prop_name: string):` <mark style="color:purple;">`entity`</mark>

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
{% endtab %}

{% tab title="vector" %}
`<entity>:get_prop_vector(class_name: string, prop_name: string):` <mark style="color:purple;">`vector`</mark>

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
{% endtab %}
{% endtabs %}

## Setting prop values

{% tabs %}
{% tab title="int" %}
`<entity>:set_prop_int(class_name: string, prop_name: string, value: number)`

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
| **value**       | **`number`** | Prop value  |
{% endtab %}

{% tab title="float" %}
`<entity>:set_prop_float(class_name: string, prop_name: string, value: number)`

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
| **value**       | **`number`** | Prop value  |
{% endtab %}

{% tab title="bool" %}
`<entity>:set_prop_bool(class_name: string, prop_name: string, value: boolean)`

| Name            | Type          | Description |
| --------------- | ------------- | ----------- |
| **class\_name** | **`string`**  | Class name  |
| **prop\_name**  | **`string`**  | Prop name   |
| **value**       | **`boolean`** | Prop value  |
{% endtab %}

{% tab title="string" %}
`<entity>:set_prop_string(class_name: string, prop_name: string, value: string)`

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
| **value**       | **`string`** | Prop value  |
{% endtab %}

{% tab title="entity" %}
`<entity>:set_prop_entity(class_name: string, prop_name: string, value: string)`

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
| **value**       | **`entity`** | Prop value  |
{% endtab %}

{% tab title="vector" %}
`<entity>:set_prop_vector(class_name: string, prop_name: string, value: vector)`

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **class\_name** | **`string`** | Class name  |
| **prop\_name**  | **`string`** | Prop name   |
| **value**       | **`vector`** | Prop value  |
{% endtab %}
{% endtabs %}
