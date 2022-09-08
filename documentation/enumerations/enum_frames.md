# 🎞 enum\_frames

| Name                                        |
| ------------------------------------------- |
| **`frame_start`**                           |
| **`frame_net_update_start`**                |
| **`frame_net_update_end`**                  |
| **`frame_net_update_postdataupdate_start`** |
| **`frame_net_update_postdataupdate_end`**   |
| **`frame_render_start`**                    |
| **`frame_render_end`**                      |

```lua
cheat.push_callback("on_frame_net", function(stage)
    if (stage == enum_frames.frame_start) then
        cheat.notify("frame_start")
    end
end)
```
