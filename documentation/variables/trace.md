# ✈ trace

## Functions:

### ray

`trace.ray(vec_start: vector, vec_end: vector, skip_entity: entity, mask: number):` <mark style="color:purple;">`trace`</mark>

| Name             | Type         | Description                  |
| ---------------- | ------------ | ---------------------------- |
| **vec\_start**   | **`vector`** | Vector to start tracing from |
| **vec\_end**     | **`vector`** | Vector to trace to           |
| **skip\_entity** | **`entity`** | Entity skipping options      |
| **mask**         | **`number`** | Trace mask                   |

```lua
local trace_example = trace.ray(vector(0,0,0), vector(100, 100, 100), entity.get_local(), 0xFFFFFFFF)
local trace_fraction = trace_example.fraction
```

Returns a [`trace`](trace.md#struct-trace) struct containing all the information.

#### 🔗 struct <mark style="color:blue;">`trace`</mark>

| Name            | Type         | Description                                                                                                                                        |
| --------------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| **fraction**    | **`number`** | Percentage in the range \[0.0, 1.0]. How far the trace went before hitting something. <mark style="color:blue;">`1.0`</mark> - didn't hit anything |
| **hit\_entity** | **`entity`** | Entity that was hit by the trace                                                                                                                   |
| **hitgroup**    | **`number`** | <mark style="color:blue;">`0`</mark> - generic, non-zero is specific body part                                                                     |
| **endpos**      | **`vector`** | Final position                                                                                                                                     |
