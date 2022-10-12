# 🌎 globalvars

## Functions:

### get\_menu

`globalvars.get_menu():` <mark style="color:purple;">`vector_4d`</mark>

<mark style="color:blue;">`x`</mark> - Menu position on the X axis.\
<mark style="color:blue;">`y`</mark> - Menu position on the Y axis.\
<mark style="color:blue;">`z`</mark> - Menu width.\
<mark style="color:blue;">`h`</mark> - Menu height.

Returns menu options.

### is\_open\_menu

`globalvars.is_open_menu():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the menu is open.

### get\_framerate

`globalvars.get_framerate():` <mark style="color:purple;">`number`</mark>

Returns the number of frames.

### get\_ping

`globalvars.get_ping():` <mark style="color:purple;">`number`</mark>

Returns the ping of the local player.

### get\_server\_address

`globalvars.get_server_address():` <mark style="color:purple;">`string`</mark>

Returns the server ip.

### get\_time

`globalvars.get_time():` <mark style="color:purple;">`string`</mark>

Returns the time specified on the computer.

### get\_winuser

`globalvars.get_winuser():` <mark style="color:purple;">`string`</mark>

Returns the computer user name.

### get\_realtime

`globalvars.get_realtime():` <mark style="color:purple;">`number`</mark>

Returns the local time in seconds.

### get\_curtime

`globalvars.get_curtime():` <mark style="color:purple;">`number`</mark>

Returns the server time in seconds.

### get\_frametime

`globalvars.get_frametime():` <mark style="color:purple;">`number`</mark>

Returns the duration of the last game frame in seconds.

### get\_absolute\_frametime

`globalvars.get_absolute_frametime():` <mark style="color:purple;">`number`</mark>

Returns the duration of the last game frame in seconds.

### get\_tickcount

`globalvars.get_tickcount():` <mark style="color:purple;">`number`</mark>

Returns the number of ticks elapsed on the server.

### get\_framecount

`globalvars.get_framecount():` <mark style="color:purple;">`number`</mark>

Returns the amount of frames since the game started.

### get\_intervalpertick

`globalvars.get_intervalpertick():` <mark style="color:purple;">`number`</mark>

Returns the duration of a tick in seconds.

### get\_maxclients

`globalvars.get_maxclients():` <mark style="color:purple;">`number`</mark>

Returns the maximum number of players on the server.

### get\_dt\_recharging

`globalvars.get_dt_recharging():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:red;">`false`</mark>, if double tap is charged.

### get\_spectators

`globalvars.get_spectators():` <mark style="color:purple;">`table`</mark>

Returns a table of pointers to the players that are currently spectating the local player.
