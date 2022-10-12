# 🖥 console

## Functions:

### execute\_client\_cmd

`console.execute_client_cmd(command: string)`

| Name        | Type         | Description |
| ----------- | ------------ | ----------- |
| **command** | **`string`** | command     |

Executes a ConCommand.

### print

`console.print(message: string)`

| Name        | Type         | Description |
| ----------- | ------------ | ----------- |
| **message** | **`string`** | message     |

Outputs text to the console.

### print\_color

`console.print_color(message: string, message_color: color)`

| Name               | Type         | Description    |
| ------------------ | ------------ | -------------- |
| **message**        | **`string`** | message        |
| **message\_color** | **`color`**  | message\_color |

Outputs text to the console with a specific color.

### get\_int

`console.get_int(name: string):` <mark style="color:purple;">`number`</mark>

Returns the ConVar int value.

### get\_float

`console.get_float(name: string):` <mark style="color:purple;">`number`</mark>

Returns the ConVar float value.

### get\_bool

`console.get_bool(name: string):` <mark style="color:purple;">`boolean`</mark>

Returns the ConVar boolean value.

### get\_string

`console.get_string(name: string):` <mark style="color:purple;">`string`</mark>

Returns the ConVar string value.

### set\_int

`console.set_int(name: string, var: number)`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | -           |
| **var**  | **`number`** | -           |

Sets the ConVar int value.

### set\_float

`console.set_float(name: string, var: number)`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | -           |
| **var**  | **`number`** | -           |

Sets the ConVar float value.

### set\_bool

`console.set_bool(name: string, var: boolean)`

| Name     | Type          | Description |
| -------- | ------------- | ----------- |
| **name** | **`string`**  | -           |
| **var**  | **`boolean`** | -           |

Sets the ConVar boolean value.

### set\_string

`console.set_string(name: string, var: string)`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | -           |
| **var**  | **`string`** | -           |

Sets the ConVar string value.
