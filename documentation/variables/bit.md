# 📠 bit

## Functions:

### band

`bit.band(a: number, b: number):` <mark style="color:purple;">`number`</mark>

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **a** | **`number`** | a           |
| **b** | **`number`** | b           |

Returns the bitwise and of all of its arguments.

### bnot

`bit.bnot(a: number):` <mark style="color:purple;">`number`</mark>

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **a** | **`number`** | a           |

Returns the bitwise not of its argument.

### lshift

`bit.lshift(a: number, b: number):` <mark style="color:purple;">`number`</mark>

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **a** | **`number`** | a           |
| **b** | **`number`** | b           |

Returns the bitwise logical left-shift of its first argument by the number of bits given by the second argument. Logical shifts treat the first argument as an unsigned number and shift in 0-bits. Only the lower 5 bits of the shift count are used (reduces to the range \[0..31]).

### rshift

`bit.rshift(a: number, b: number):` <mark style="color:purple;">`number`</mark>

| Name  | Type         | Description |
| ----- | ------------ | ----------- |
| **a** | **`number`** | a           |
| **b** | **`number`** | b           |

Returns the bitwise logical right-shift of its first argument by the number of bits given by the second argument. Logical shifts treat the first argument as an unsigned number and shift in 0-bits. Only the lower 5 bits of the shift count are used (reduces to the range \[0..31]).
