# 🧱 materials

## Functions:

### get\_material\_by\_name

`materials.get_material_by_name(path: string):` <mark style="color:purple;">`material`</mark>

| Name     | Type         | Description                         |
| -------- | ------------ | ----------------------------------- |
| **path** | **`string`** | Directory to the specified material |

Returns the material object in the specified path.

### get\_first\_material

`materials.get_first_material():` <mark style="color:purple;">`material`</mark>

Returns the first material.

### get\_next\_material

`materials.get_next_material(mat: material):` <mark style="color:purple;">`material`</mark>

| Name    | Type           | Description |
| ------- | -------------- | ----------- |
| **mat** | **`material`** | -           |

Returns the next material.

### get\_material

`materials.get_material(mat: material):` <mark style="color:purple;">`material`</mark>

| Name    | Type           | Description |
| ------- | -------------- | ----------- |
| **mat** | **`material`** | -           |

Returns the material.

### get\_material\_name

`materials.get_material_name(mat: material):` <mark style="color:purple;">`string`</mark>

| Name    | Type           | Description |
| ------- | -------------- | ----------- |
| **mat** | **`material`** | -           |

Returns the name of the material.

### set\_material\_var\_flag

`materials.set_material_var_flag(mat: material, flag: number, state: boolean)`

| Name      | Type           | Description |
| --------- | -------------- | ----------- |
| **mat**   | **`material`** | -           |
| **flag**  | **`number`**   | -           |
| **state** | **`boolean`**  | -           |

Sets the value of the material var flag.

### color\_modulate

`materials.color_modulate(mat: material, clr: color)`

| Name    | Type           | Description |
| ------- | -------------- | ----------- |
| **mat** | **`material`** | -           |
| **clr** | **`color`**    | -           |

&#x20;Sets the material color modulation value.

### set\_alpha

`materials.set_alpha(mat: material, alpha: number)`

| Name      | Type           | Description |
| --------- | -------------- | ----------- |
| **mat**   | **`material`** | -           |
| **alpha** | **`number`**   | -           |

Sets the material alpha modulation value.
