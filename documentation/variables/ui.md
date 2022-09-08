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

## Combobox functions:

### :set_items()

`<element>:set_items(items: { , ... }):` <mark style="color:purple;">`items: string`</mark>
`Sets items for combobox element`

### :get_items()

`<element>:get_items():` <mark style="color:purple;">`items: string`</mark>
`Returns items from combobox element`
