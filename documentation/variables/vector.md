# ⚡ vector

## Variables:

{% tabs %}
{% tab title="vector" %}
`vector(x: number, y: number, z: number)`

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **x** | **`number`** | -           |
| **y** | **`number`** | -           |
| **z** | **`number`** | -           |

**How to use vector:**

```lua
--> Vectors
local new_vec = vector(255, 255, 255)
local sec_vec = vector(2000, 100, 100)

--> Length
local new_vec_length = new_vec:length()

--> Distance
local dist = new_vec:dist_to(sec_vec)
```

####

#### Functions:

#### :length

`vec_object:length():` <mark style="color:purple;">`number`</mark>

Returns the length of the vector.

#### :length\_sqr

`vec_object:length_sqr():` <mark style="color:purple;">`number`</mark>

Returns the squared length of the vector.

#### :length\_2d

`vec_object:length_2d():` <mark style="color:purple;">`number`</mark>

Returns the length of the vector in two dimensions, without the Z axis.

#### :length\_2d\_sqr

`vec_object:length_2d_sqr():` <mark style="color:purple;">`number`</mark>

Returns the squared length of the vectors x and y value.

#### :is\_zero

`vec_object:is_zero():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if all coordinates of the vector are zero.

#### :is\_valid

`vec_object:is_valid():` <mark style="color:purple;">`boolean`</mark>

Returns <mark style="color:green;">`true`</mark>, if the vector is valid.

#### :zero

`vec_object:zero():` <mark style="color:purple;">`vector`</mark>

Sets zero values to the vector.

#### :dist\_to

`vec_object:dist_to(vec_end: vector):` <mark style="color:purple;">`number`</mark>

| Name         | Type         | Description                       |
| ------------ | ------------ | --------------------------------- |
| **vec\_end** | **`vector`** | The vector to get the distance to |

Returns the distance between the two given vectors.

#### :dist\_to\_sqr

`vec_object:dist_to_sqr(vec_end: vector):` <mark style="color:purple;">`number`</mark>

| Name         | Type         | Description                               |
| ------------ | ------------ | ----------------------------------------- |
| **vec\_end** | **`vector`** | The vector to get the squared distance to |

Returns the squared distance to another vector.

#### :cross\_product

`vec_object:cross_product(vec_end: vector):` <mark style="color:purple;">`vector`</mark>

| Name         | Type         | Description                                    |
| ------------ | ------------ | ---------------------------------------------- |
| **vec\_end** | **`vector`** | The vector to calculate the cross product with |

Returns the cross product of two given vectors.

#### :normalize

`vec_object:normalize():` <mark style="color:purple;">`number`</mark>

Normalizes the vector and returns the length of the vector.
{% endtab %}

{% tab title="vector_2d" %}
`vector_2d(x: number, y: number)`

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **x** | **`number`** | -           |
| **y** | **`number`** | -           |

**How to use vector\_2d:**

```lua
--> Vectors
local new_vec = vector_2d(255, 255)

--> Output info
cheat.notify(new_vec.x .. new_vec.y)
```
{% endtab %}

{% tab title="vector_4d" %}
`vector_4d(x: number, y: number, z: number, w: number)`

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **x** | **`number`** | -           |
| **y** | **`number`** | -           |
| **z** | **`number`** | -           |
| **w** | **`number`** | -           |

**How to use vector\_4d:**

```lua
--> Vectors 
local new_vec = vector_4d(255, 255, 255, 255)

--> Output info 
cheat.notify(new_vec.x .. new_vec.y .. new_vec.z .. new_vec.w)
```
{% endtab %}
{% endtabs %}
