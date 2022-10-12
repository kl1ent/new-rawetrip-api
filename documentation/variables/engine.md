# 🛠 engine

## Functions:

### get\_screen\_size

`engine.get_screen_size():` <mark style="color:purple;">`vector`</mark>

Returns the screen size.

### get\_level\_name

`engine.get_level_name():` <mark style="color:purple;">`string`</mark>

### get\_level\_name\_short

`engine.get_level_name_short():` <mark style="color:purple;">`string`</mark>

### get\_map\_group\_name

`engine.get_map_group_name():` <mark style="color:purple;">`string`</mark>

Returns the map group.

### get\_local\_player\_index

`engine.get_local_player_index():` <mark style="color:purple;">`number`</mark>

Returns the index of the local player.

### get\_player\_for\_user\_id

`engine.get_player_for_user_id(userid: number):` <mark style="color:purple;">`entity`</mark>

| Name       | Type         | Description |
| ---------- | ------------ | ----------- |
| **userid** | **`number`** | User id     |

Returns a pointer to the specified player.

### get\_view\_angles

`engine.get_view_angles():` <mark style="color:purple;">`vector`</mark>

Returns the player view angles.

### is\_connected

`engine.is_connected():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the player is connected.

### is\_hltv

`engine.is_hltv():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the is hltv.

### is\_paused

`engine.is_paused():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the game is paused.

### is\_in\_game

`engine.is_in_game():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the player is currently connected to a game server.

### is\_playing\_demo

`engine.is_playing_demo():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the demo is being played.

### is\_recording\_demo

`engine.is_recording_demo():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the demo is being recorded.

### is\_taking\_screenshot

`engine.is_taking_screenshot():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if a screenshot was taken.

### is\_voice\_recording

`engine.is_voice_recording():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if you are speaking in voice chat.

### set\_view\_angles

`engine.set_view_angles(angles: vector)`

| Name       | Type         | Description   |
| ---------- | ------------ | ------------- |
| **angles** | **`vector`** | Player angles |

Sets view angles to the player.

### set\_clantag

`engine.set_clantag(tag: string)`

| Name    | Type         | Description |
| ------- | ------------ | ----------- |
| **tag** | **`string`** | Clan tag    |

Sets your in-game clan tag.

### get\_gamename

`engine.get_gamename():` <mark style="color:purple;">`string`</mark>

Returns the game name.

### get\_winpath

`engine.get_winpath(type: string)`

| Name     | Type         | Description                                         |
| -------- | ------------ | --------------------------------------------------- |
| **type** | **`string`** | Types: <mark style="color:purple;">`appdata`</mark> |

Returns a specific path.

### get\_gamepath

`engine.get_gamepath():` <mark style="color:purple;">`string`</mark>

Returns the path to the game client folder.

### get\_roundstart\_time

`engine.get_roundstart_time():` <mark style="color:purple;">`number`</mark>

Returns the time before the start of the round.

### get\_round\_time

`engine.get_round_time():` <mark style="color:purple;">`number`</mark>

Returns the time of the round.
