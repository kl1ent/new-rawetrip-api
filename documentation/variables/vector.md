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

#### How to use vector:

```lua
--> Vectors
local new_vec = vector(255, 255, 255)
local sec_vec = vector(2000, 100, 100)

--> Length
local new_vec_length = new_vec:length()

--> Distance
local dist = new_vec:dist_to(sec_vec)
```

###

### Functions:
{% endtab %}

{% tab title="vector_2d" %}
`vector(x: number, y: number)`

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **x** | **`number`** | -           |
| **y** | **`number`** | -           |

#### How to use vector\_2d:

```lua
--> Vectors
local new_vec = vector_2d(255, 255)

--> Output info
cheat.notify(new_vec.x .. new_vec.y)
```
{% endtab %}

{% tab title="vector_4d" %}
`vector(x: number, y: number, z: number, w: number)`

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **x** | **`number`** | -           |
| **y** | **`number`** | -           |
| **z** | **`number`** | -           |
| **w** | **`number`** | -           |

#### How to use vector\_4d:

```lua
--> Vectors 
local new_vec = vector_2d(255, 255, 255, 255)

--> Output info 
cheat.notify(new_vec.x .. new_vec.y .. new_vec.z .. new_vec.w)
```
{% endtab %}
{% endtabs %}

|       |              |   |
| ----- | ------------ | - |
| **x** | **`number`** | - |
| **y** | **`number`** | - |
| **z** | **`number`** | - |

## How to use vector:

```lua
--> Vectors
local new_vec = vector(255, 255, 255)
local sec_vec = vector(2000, 100, 100)

--> Length
local new_vec_length = new_vec:length()

--> Distance
local dist = new_vec:dist_to(sec_vec)
```

## Functions:

### :length

`vec_object:length():` <mark style="color:purple;">`number`</mark>

### :length\_sqr

`vec_object:length_sqr():` <mark style="color:purple;">`number`</mark>

### :length\_2d

`vec_object:length_2d():` <mark style="color:purple;">`number`</mark>

### :length\_2d\_sqr

`vec_object:length_2d_sqr():` <mark style="color:purple;">`number`</mark>

### :is\_zero

`vec_object:is_zero():` <mark style="color:purple;">`boolean`</mark>

### :is\_valid

`vec_object:is_valid():` <mark style="color:purple;">`boolean`</mark>

### :zero

`vec_object:zero():` <mark style="color:purple;">`vector`</mark>

### :dist\_to

`vec_object:dist_to(vec_end: vector):` <mark style="color:purple;">`number`</mark>

| Name         | Type         | Description                       |
| ------------ | ------------ | --------------------------------- |
| **vec\_end** | **`vector`** | The vector to get the distance to |

### :dist\_to\_sqr

`vec_object:dist_to_sqr(vec_end: vector):` <mark style="color:purple;">`number`</mark>

| Name         | Type         | Description                               |
| ------------ | ------------ | ----------------------------------------- |
| **vec\_end** | **`vector`** | The vector to get the squared distance to |

### :cross\_product

`vec_object:cross_product(vec_end: vector):` <mark style="color:purple;">`vector`</mark>

| Name         | Type         | Description                                    |
| ------------ | ------------ | ---------------------------------------------- |
| **vec\_end** | **`vector`** | The vector to calculate the cross product with |

### :normalize

`vec_object:normalize():` <mark style="color:purple;">`number`</mark>
