# 🏙 render

## Functions:

### world\_to\_screen

`render.world_to_screen(position: vector):` <mark style="color:purple;">`vector`</mark>

| Name         | Type         | Description             |
| ------------ | ------------ | ----------------------- |
| **position** | **`vector`** | Position in world space |

Returns the screen position vector. This can only be called from the on\_paint callback.

### setup\_font

`render.setup_font(name: string, size: number, flags: number):` <mark style="color:purple;">`FontObject`</mark>

| Name      | Type         | Description                                                                                                                                                                                                                                                                                                                                                          |
| --------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **name**  | **`string`** | Font that will be initialized                                                                                                                                                                                                                                                                                                                                        |
| **size**  | **`number`** | Size of the font                                                                                                                                                                                                                                                                                                                                                     |
| **flags** | **`number`** | <mark style="color:purple;">`fontflags.noantialiasing`</mark> <mark style="color:purple;"></mark><mark style="color:purple;"></mark> for anti-aliasing, <mark style="color:purple;">`fontflags.italic`</mark> <mark style="color:purple;"></mark><mark style="color:purple;"></mark> for cursive text, <mark style="color:purple;">`fontflags.bold`</mark> bold text |

```lua
local font = render.setup_font("Verdana", 12, fontflags.noantialiasing | fontflags.bold)
```

Returns the <mark style="color:purple;">`FontObject`</mark> struct or nil on failure.

### setup\_weapon\_font

`render.setup_weapon_font(size: number):` <mark style="color:purple;">`FontObject`</mark>

| Name     | Type         | Description      |
| -------- | ------------ | ---------------- |
| **size** | **`number`** | Size of the font |

Returns the <mark style="color:purple;">`FontObject`</mark> struct or nil on failure.

### setup\_texture

`render.setup_texture(path: string):` <mark style="color:purple;">`texture`</mark>

| Name                                        | Type     | Description       |
| ------------------------------------------- | -------- | ----------------- |
| <mark style="color:purple;">**path**</mark> | `string` | Path to the image |

Returns the <mark style="color:purple;">`texture`</mark> <mark style="color:purple;"></mark><mark style="color:purple;"></mark> or nil on failure.

### get\_text\_size

`render.get_text_size(font: FontObject, text: string):` <mark style="color:purple;">`vector`</mark>

| Name     | Type             | Description                |
| -------- | ---------------- | -------------------------- |
| **font** | **`FontObject`** | Font                       |
| **text** | **`string`**     | Text that will be measured |

Returns the size of the text.

## Structs

### 🔗 <mark style="color:blue;">`FontObject`</mark>

#### size

`font.size:` <mark style="color:purple;">`number`</mark>

## Draw functions

### blur

`render.blur(x: number, y: number: width: number, height: number, alpha: number)`

| Name       | Type         | Description                             |
| ---------- | ------------ | --------------------------------------- |
| **x**      | **`number`** | X position                              |
| **y**      | **`number`** | Y position                              |
| **width**  | **`number`** | Width                                   |
| **height** | **`number`** | Height                                  |
| **alpha**  | **`number`** | Alpha percentage in the range \[0, 255] |

### line

`render.line(x: number, y: number, x2: number, y2: number, color: color, thickness: number)`

| Name          | Type         | Description           |
| ------------- | ------------ | --------------------- |
| **x**         | **`number`** | X position            |
| **y**         | **`number`** | Y position            |
| **x2**        | **`number`** | X2 position           |
| **y2**        | **`number`** | Y2 position           |
| **color**     | **`color`**  | Color of the line     |
| **thickness** | **`number`** | Thickness of the line |

### polygon

`render.polygon(color: color, positions: {, ...})`

|               |              |                      |
| ------------- | ------------ | -------------------- |
| **color**     | **`color`**  | Color of the polygon |
| **positions** | **`vector`** | Screen positions     |

### polyline

`render.polyline(color: color, closed: boolean, thickness: number, positions: {, ...})`

|               |               |                           |
| ------------- | ------------- | ------------------------- |
| **color**     | **`color`**   | Color of the polyline     |
| **closed**    | **`boolean`** | -                         |
| **thickness** | **`number`**  | Thickness of the polyline |
| **positions** | **`vector`**  | Screen positions          |

### rect

`render.rect(x: number, y: number, width: number, height: number, color: color[, rounding: number])`

| Name         | Type         | Description                                   |
| ------------ | ------------ | --------------------------------------------- |
| **x**        | **`number`** | X position                                    |
| **y**        | **`number`** | Y position                                    |
| **width**    | **`number`** | Width                                         |
| **height**   | **`number`** | Height                                        |
| **color**    | **`color`**  | Color of the rectangle                        |
| **rounding** | **`number`** | Optional. Rounding of the rectangle in pixels |

### rect\_filled

`render.rect_filled(x: number, y: number, width: number, height: number, color: color[, rounding: number])`

| Name         | Type         | Description                                   |
| ------------ | ------------ | --------------------------------------------- |
| **x**        | **`number`** | X position                                    |
| **y**        | **`number`** | Y position                                    |
| **width**    | **`number`** | Width                                         |
| **height**   | **`number`** | Height                                        |
| **color**    | **`color`**  | Color of the rectangle                        |
| **rounding** | **`number`** | Optional. Rounding of the rectangle in pixels |

### gradient

`render.gradient(x: number, y: number, width: number, height: number, first_color: color, second_color[, type: number])`

| Name              | Type         | Description                                                                                                      |
| ----------------- | ------------ | ---------------------------------------------------------------------------------------------------------------- |
| **x**             | **`number`** | X position                                                                                                       |
| **y**             | **`number`** | Y position                                                                                                       |
| **width**         | **`number`** | Width                                                                                                            |
| **height**        | **`number`** | Height                                                                                                           |
| **first\_color**  | **`color`**  | First color                                                                                                      |
| **second\_color** | **`color`**  | Second color                                                                                                     |
| **type**          | **`number`** | Optional. <mark style="color:purple;">`0`</mark> - horizontal, <mark style="color:purple;">`1`</mark> - vertical |

### circle

`render.circle(x: number, y: number, points: number, radius: number, color: color)`

| Name       | Type         | Description          |
| ---------- | ------------ | -------------------- |
| **x**      | **`number`** | X position           |
| **y**      | **`number`** | Y position           |
| **points** | **`number`** | Points of the circle |
| **radius** | **`number`** | Radius of the circle |
| **color**  | **`color`**  | Color of the circle  |

### circle\_filled

`render.circle_filled(x: number, y: number, points: number, radius: number, color: color)`

| Name       | Type         | Description          |
| ---------- | ------------ | -------------------- |
| **x**      | **`number`** | X position           |
| **y**      | **`number`** | Y position           |
| **points** | **`number`** | Points of the circle |
| **radius** | **`number`** | Radius of the circle |
| **color**  | **`color`**  | Color of the circle  |

### glow\_circle

`render.glow_circle(x: number, y: number, radius: number, color: color)`

| Name       | Type         | Description          |
| ---------- | ------------ | -------------------- |
| **x**      | **`number`** | X position           |
| **y**      | **`number`** | Y position           |
| **radius** | **`number`** | Radius of the circle |
| **color**  | **`color`**  | Color of the circle  |

### arc

`render.arc(x: number, y: number: radius: number, second_radius: number, min: number, max: number, color: color)`

| Name               | Type         | Description                 |
| ------------------ | ------------ | --------------------------- |
| **x**              | **`number`** | X position                  |
| **y**              | **`number`** | Y position                  |
| **radius**         | **`number`** | Radiusof the circle         |
| **second\_radius** | **`number`** | Second radius of the circle |
| **min**            | **`number`** | Minimum value               |
| **max**            | **`number`** | Maximum value               |
| **color**          | **`color`**  | Color of the circle         |

### circle\_3d

`render.circle_3d(position: vector, radius: number, color: color)`

| Name         | Type         | Description          |
| ------------ | ------------ | -------------------- |
| **position** | **`vector`** | Screen position      |
| **radius**   | **`number`** | Radius of the circle |
| **color**    | **`color`**  | Color of the circle  |

### circle\_filled\_3d

`render.circle_filled_3d(position: vector, radius: number, color: color)`

| Name         | Type         | Description          |
| ------------ | ------------ | -------------------- |
| **position** | **`vector`** | Screen position      |
| **radius**   | **`number`** | Radius of the circle |
| **color**    | **`color`**  | Color of the circle  |

### text

📌 Render any text via the [`:setup_font`](render.md#setup\_font) or [`:setup_weapon_font`](render.md#setup\_weapon\_font) function.

`render.text(font: FontObject, x: number, y: number, color: color, text: string[, shadow: boolean, outline: boolean])`

| Name        | Type             | Description             |
| ----------- | ---------------- | ----------------------- |
| **font**    | **`FontObject`** | Font                    |
| **x**       | **`number`**     | X position              |
| **y**       | **`number`**     | Y position              |
| **color**   | **`color`**      | Color of the text       |
| **text**    | **`string`**     | Text that will be drawn |
| **shadow**  | **`boolean`**    | Optional. Text shadow   |
| **outline** | **`boolean`**    | Optional. Text outline  |

### image

`render.image(texture: texture, x: number, y: number, width: number, height: number, color: color[, rounding: number])`

| Name         | Type          | Description              |
| ------------ | ------------- | ------------------------ |
| **texture**  | **`texture`** | Texture                  |
| **x**        | **`number`**  | X position               |
| **y**        | **`number`**  | Y position               |
| **width**    | **`number`**  | Width                    |
| **height**   | **`number`**  | Height                   |
| **color**    | **`color`**   | Color of the image       |
| **rounding** | **`number`**  | Optional. Image rounding |

### rect\_shadow

`render.rect_shadow(x: number, y: number, width: number, height: number, length: number, color: color[, x_offset: number, y_offset: number])`

| Name          | Type         | Description         |
| ------------- | ------------ | ------------------- |
| **x**         | **`number`** | X position          |
| **y**         | **`number`** | Y position          |
| **width**     | **`number`** | Width               |
| **height**    | **`number`** | Height              |
| **length**    | **`number`** | Shadow length       |
| **color**     | **`color`**  | Color of the shadow |
| **x\_offset** | **`number`** | Optional. X offset  |
| **y\_offset** | **`number`** | Optional. Y offset  |

### begin\_cliprect

`render.begin_cliprect(x: number, y: number, width: number, height: number)`

| Name       | Type         | Description |
| ---------- | ------------ | ----------- |
| **x**      | **`number`** | X position  |
| **y**      | **`number`** | Y position  |
| **width**  | **`number`** | Width       |
| **height** | **`number`** | Height      |

Applies the clip region to the given rectangle for all subsequent elements.

### end\_cliprect

`render.end_cliprect()`

Discards an early set rectangle clipping region.
