# ✈ trace

## Functions:

### ray

`trace.ray(vec_start: vector, vec_end: vector, skip_entity: entity, mask: number):` <mark style="color:purple;">`table`</mark>

| Name             | Type         | Description |
| ---------------- | ------------ | ----------- |
| **vec\_start**   | **`vector`** | -           |
| **vec\_end**     | **`vector`** | -           |
| **skip\_entity** | **`entity`** | -           |
| **mask**         | **`number`** | -           |

```lua
local trace_example = trace.ray(vector(0,0,0), vector(100, 100, 100), entity.get_local(), 0xFFFFFFFF)
local trace_fraction = trace_example.fraction
```

| Name            | Type         | Description |
| --------------- | ------------ | ----------- |
| **fraction**    | **`number`** | -           |
| **hit\_entity** | **`entity`** | -           |
| **hitgroup**    | **`number`** | -           |
| **endpos**      | **`vector`** | -           |
