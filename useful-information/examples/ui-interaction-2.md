# ⚙ Wireframe smoke

### Example of wireframe smoke

{% hint style="info" %}
To do something like this, you can refer to the [materials.md](../../documentation/variables/materials.md "mention")
{% endhint %}

```lua
local smokeMaterials = {
    "effects/overlaysmoke",
    "particle/beam_smoke_01",
    "particle/particle_smokegrenade",
    "particle/particle_smokegrenade1",
    "particle/particle_smokegrenade2",
    "particle/particle_smokegrenade3",
    "particle/particle_smokegrenade_sc",
    "particle/smoke1/smoke1",
    "particle/smoke1/smoke1_ash",
    "particle/smoke1/smoke1_nearcull",
    "particle/smoke1/smoke1_nearcull2",
    "particle/smoke1/smoke1_snow",
    "particle/smokesprites_0001",
    "particle/smokestack",
    "particle/vistasmokev1/vistasmokev1",
    "particle/vistasmokev1/vistasmokev1_emods",
    "particle/vistasmokev1/vistasmokev1_emods_impactdust",
    "particle/vistasmokev1/vistasmokev1_fire",
    "particle/vistasmokev1/vistasmokev1_nearcull",
    "particle/vistasmokev1/vistasmokev1_nearcull_fog",
    "particle/vistasmokev1/vistasmokev1_nearcull_nodepth",
    "particle/vistasmokev1/vistasmokev1_smokegrenade",
    "particle/vistasmokev1/vistasmokev4_emods_nocull",
    "particle/vistasmokev1/vistasmokev4_nearcull",
    "particle/vistasmokev1/vistasmokev4_nocull"
}

cheat.push_callback("on_frame_net", function(stage)
    if stage ~= enum_frames.frame_render_start then
        return
    end

    for i = 0, #smokeMaterials do
        local material = materials.get_material_by_name(smokeMaterials[i])
        materials.set_material_var_flag(material, 28, true)
    end
end)
```
