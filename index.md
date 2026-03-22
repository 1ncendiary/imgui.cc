---
title: Information
icon: rel-file-path	
authors:
  - name: munyun
    avatar: https://avatars.githubusercontent.com/u/152007219?v=4
date: 2023-08-26
---

---
title: Information
icon: rel-file-path
redirect: https://imgui.cc/
---

<div align="center">
  
<img src="assets/pbc.png" width="768">

**fastflags.space** was a community-driven resource dedicated to cataloging and sharing information about FastFlags configuration.


</div>

!!!info Info
Roblox has implemented an allowlist, it limits which FastFlags can be appliedd locally in your ClientAppSettings.json file. https://devforum.roblox.com/t/allowlist-for-local-client-configuration-via-fast-flags/3966569
!!!
A method on how to bypass this via Proxy Interception is on our [Patreon](https://www.patreon.com/fastflags) (Flag Browser/Membership)

---

<div align="center">

:::content-center
[!button icon="assets/Discord-Symbol-Black.svg" size="2xl" variant="contrast" text="imgui*cc"](https://discord.gg/6zqNQTSkrg)
:::

# Whitelisted FastFlags

</div>

### Preserve rendering quality with display setting
```json
{
    "DFFlagDisableDPIScale": "True"
}
```
### FRM Quality Levels
> [!TIP]
> **1-6 Are low graphics, Above 6 are high graphics**
```json
{
    "DFIntDebugFRMQualityLevelOverride": "1"
}
```
### Pause Voxelizer/Disable Baked Shadows
```json
{
    "DFFlagDebugPauseVoxelizer": "True"
}
```
### Gray Sky
> [!IMPORTANT]
> **Only applies to games with the default skybox**
```json
{
    "FFlagDebugSkyGray": "True"
}
```
### Force LOD on Meshes
```json
{
    "DFIntCSGLevelOfDetailSwitchingDistance": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0"
}
```
### Force Texture Quality 
> [!TIP]
> **Set any value from 0-3**
```json
{
    "DFFlagTextureQualityOverrideEnabled": "True",
    "DFIntTextureQualityOverride": "3"
}
```
### Remove Grass
```json
{
    "FIntFRMMinGrassDistance": "0",
    "FIntFRMMaxGrassDistance": "0",
    "FIntRenderGrassDetailStrands": "0",
}
```
### Force MSAA 
> [!IMPORTANT]
> **Values: 0, 1, 2, 4, 8**

> [!CAUTION]
> **Values over 4> will cause viewport bugs**
```json
{
    "FIntDebugForceMSAASamples": "4"
}
```
### Increased Grass Motion & No Grass Motion
```json
{
    "FIntGrassMovementReducedMotionFactor": "999"
}
```
```json
{
    "FIntGrassMovementReducedMotionFactor": "0"
}
```
### Exclusive Fullscreen
> [!TIP]
> Alt + Delete
```json
{
    "FFlagHandleAltEnterFullscreenManually": "False"
}
```
