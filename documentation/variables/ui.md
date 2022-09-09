# 💻 ui

## Elements:

### add\_checkbox

`ui.add_checkbox(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

### add\_combobox

`ui.add_combobox(name: string, items: { , ... }):` <mark style="color:purple;">`MenuItem`</mark>

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **name**  | **`string`** | Item name   |
| **items** | **`string`** | Items       |

### add\_sliderint

`ui.add_sliderint(name: string, min: number, max: number):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description   |
| -------- | ------------ | ------------- |
| **name** | **`string`** | Item name     |
| **min**  | **`number`** | Minimum value |
| **max**  | **`number`** | Maximum value |

### add\_sliderfloat

`ui.add_sliderfloat(name: string, min: number, max: number):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description   |
| -------- | ------------ | ------------- |
| **name** | **`string`** | Item name     |
| **min**  | **`number`** | Minimum value |
| **max**  | **`number`** | Maximum value |

### add\_button

`ui.add_button(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

### add\_colorpicker

`ui.add_colorpicker(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

### add\_label

`ui.add_label(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

### add\_hotkey

`ui.add_hotkey(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

### get\_keybind\_state

`ui.get_keybind_state(name: string)`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Returns hotkey state from menu

### get\_keybind\_mode

`ui.get_keybind_mode(name: string)`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Returns hotkey mode from menu

### set\_keybind\_state

`ui.set_keybind_state(name: string, var: boolean)`

| Name     | Type          | Description |
| -------- | ------------- | ----------- |
| **name** | **`string`**  | Item name   |
| **var**  | **`boolean`** | Item var    |

Sets hotkey state from menu

## Functions:

### :get

`<element>:get():` <mark style="color:purple;">`any`</mark>&#x20;

Returns the value received from the element

### :set

`<element>:set(value: any)`&#x20;

| Name      | Type      | Description                                  |
| --------- | --------- | -------------------------------------------- |
| **value** | **`any`** | The value to which the menu item will be set |

Sets your value

### :set\_visible

`<element>:set_visible(state: boolean)`

| Name      | Type          | Description          |
| --------- | ------------- | -------------------- |
| **state** | **`boolean`** | New visibility state |

Sets the visibility of the element

## Combobox additive functions:

### :set\_items

`<element>:set_items(items: { , ... })`

| Name      | Type         | Description              |
| --------- | ------------ | ------------------------ |
| **items** | **`string`** | Table with string values |

Sets items for combobox element

### :get\_items

`<element>:get_items():` <mark style="color:purple;">`table`</mark>&#x20;

Returns items from combobox element

## Hotkey additive functions:

### :get\_mode

`<element>:get_mode():` <mark style="color:purple;">`number`</mark>&#x20;

Returns mode from hotkey element
