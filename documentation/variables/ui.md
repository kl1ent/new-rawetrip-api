# 💻 ui

## Elements:

### add_checkbox

`ui.add_checkbox(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |

### add_combobox

`ui.add_combobox(name: string, items: { , ... }):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |
| **items** | **`String`** | Items   |

### add_sliderint

`ui.add_sliderint(name: string, min: number, max: number):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |
| **min** | **`Number`** | Minimum value   |
| **max** | **`Number`** | Maximum value   |

### add_sliderfloat

`ui.add_sliderfloat(name: string, min: number, max: number):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |
| **min** | **`Number`** | Minimum value   |
| **max** | **`Number`** | Maximum value   |

### add_button

`ui.add_button(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |

### add_colorpicker

`ui.add_colorpicker(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |

### add_label

`ui.add_label(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |

### add_hotkey

`ui.add_hotkey(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |

### get_keybind_state

`ui.get_keybind_state(name: string):` `Returns hotkey state from menu`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |

### get_keybind_mode

`ui.get_keybind_mode(name: string):` `Returns hotkey mode from menu`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |

### set_keybind_state

`ui.set_keybind_state(name: string, var: boolean):` `Sets hotkey state from menu`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`String`** | Item name   |
| **var** | **`Boolean`** | Item var   |

## Functions:

### :get()

`<element>:get():` <mark style="color:purple;">`boolean/number`</mark>
`Returns the value received from the element`

### :set()

`<element>:set(var: boolean/number):` <mark style="color:purple;">`boolean/number`</mark>
`Sets your value`

### :set_visible()

`<element>:set_visible(visible: boolean):` <mark style="color:purple;">`boolean`</mark>
`Sets the visibility of the element`

## Combobox additive functions:

### :set_items()

`<element>:set_items(items: { , ... }):` <mark style="color:purple;">`items: string`</mark>
`Sets items for combobox element`

### :get_items()

`<element>:get_items():` <mark style="color:purple;">`items: string`</mark>
`Returns items from combobox element`

## Hotkey additive functions:

### :get_mode()

`<element>:get_mode():` <mark style="color:purple;">`mode: number`</mark>
`Returns mode from hotkey element`
