# 💻 ui

## Example available!

{% content-ref url="../examples/ui-interaction.md" %}
[ui-interaction.md](../examples/ui-interaction.md)
{% endcontent-ref %}

## Elements:

### add\_checkbox

`ui.add_checkbox(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Creates and returns a menu item object, or throws an error on failure.

### add\_combobox

`ui.add_combobox(name: string, items: { , ... }):` <mark style="color:purple;">`MenuItem`</mark>

| Name      | Type         | Description |
| --------- | ------------ | ----------- |
| **name**  | **`string`** | Item name   |
| **items** | **`string`** | Items       |

Creates and returns a menu item object, or throws an error on failure.

### add\_sliderint

`ui.add_sliderint(name: string, min: number, max: number):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description   |
| -------- | ------------ | ------------- |
| **name** | **`string`** | Item name     |
| **min**  | **`number`** | Minimum value |
| **max**  | **`number`** | Maximum value |

Creates and returns a menu item object, or throws an error on failure.

### add\_sliderfloat

`ui.add_sliderfloat(name: string, min: number, max: number):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description   |
| -------- | ------------ | ------------- |
| **name** | **`string`** | Item name     |
| **min**  | **`number`** | Minimum value |
| **max**  | **`number`** | Maximum value |

Creates and returns a menu item object, or throws an error on failure.

### add\_button

`ui.add_button(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Creates and returns a menu item object, or throws an error on failure.

### add\_colorpicker

`ui.add_colorpicker(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Creates and returns a menu item object, or throws an error on failure.

### add\_label

`ui.add_label(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Creates and returns a menu item object, or throws an error on failure.

### add\_hotkey

`ui.add_hotkey(name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Creates and returns a menu item object, or throws an error on failure.

### get\_keybind\_state

`ui.get_keybind_state(name: string)`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Returns <mark style="color:green;">`true`</mark>, if keybind is active.

### get\_keybind\_mode

`ui.get_keybind_mode(name: string)`

| Name     | Type         | Description |
| -------- | ------------ | ----------- |
| **name** | **`string`** | Item name   |

Returns the keybind mode.

### set\_keybind\_state

`ui.set_keybind_state(name: string, var: boolean)`

| Name     | Type          | Description |
| -------- | ------------- | ----------- |
| **name** | **`string`**  | Item name   |
| **var**  | **`boolean`** | Item var    |

Sets the keybind <mark style="color:purple;">`boolean`</mark> value.

## Functions:

### :get

`<element>:get():` <mark style="color:purple;">`any`</mark>&#x20;

Returns the value of the menu item.

### :set

`<element>:set(value: any)`&#x20;

| Name      | Type      | Description                                  |
| --------- | --------- | -------------------------------------------- |
| **value** | **`any`** | The value to which the menu item will be set |

Sets the value of the menu item.

### :set\_visible

`<element>:set_visible(state: boolean)`

| Name      | Type          | Description          |
| --------- | ------------- | -------------------- |
| **state** | **`boolean`** | New visibility state |

Shows or hides the menu item depending on the value of `state`.

## Combobox additive functions:

### :set\_items

`<element>:set_items(items: { , ... })`

| Name      | Type         | Description              |
| --------- | ------------ | ------------------------ |
| **items** | **`string`** | Table with string values |

Sets a table with items. `ui.add_combobox` menu item objects only.

### :get\_items

`<element>:get_items():` <mark style="color:purple;">`table`</mark>&#x20;

Returns the table of items. `ui.add_combobox` menu item objects only.

## Hotkey additive functions:

### :get\_mode

`<element>:get_mode():` <mark style="color:purple;">`number`</mark>&#x20;

Returns the current keybind mode. `ui.add_hotkey` menu item objects only.

## Find menu items:

{% tabs %}
{% tab title="int" %}
`ui.find_menu_int(item_name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name           | Type         | Description |
| -------------- | ------------ | ----------- |
| **item\_name** | **`string`** | -           |
{% endtab %}

{% tab title="float" %}
`ui.find_menu_float(item_name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name           | Type         | Description |
| -------------- | ------------ | ----------- |
| **item\_name** | **`string`** | -           |
{% endtab %}

{% tab title="bool" %}
`ui.find_menu_bool(item_name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name           | Type         | Description |
| -------------- | ------------ | ----------- |
| **item\_name** | **`string`** | -           |
{% endtab %}

{% tab title="color" %}
`ui.find_menu_color(item_name: string):` <mark style="color:purple;">`MenuItem`</mark>

| Name           | Type         | Description |
| -------------- | ------------ | ----------- |
| **item\_name** | **`string`** | -           |
{% endtab %}
{% endtabs %}

```lua
--> Example
local fake_lag_limit = ui.find_menu_int("Antiaim.fake_lag_limit")

fake_lag_limit:set(10)

cheat.notify(fake_lag_limit:get())
```

Returns the <mark style="color:purple;">`MenuItem`</mark> object that corresponds to the specified name.
