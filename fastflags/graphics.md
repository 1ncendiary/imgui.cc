### Set how many pixels to render
> [!NOTE]
> This does not affect performance
```json
{
    "DFIntDebugDynamicRenderKiloPixels": "1"
}
```
### Disable Highlights 
```json
{
    "DFFlagRenderHighlightManagerPrepare4": "True"
}
```
### Enable DRS
```json
{
    "FFlagRenderDynamicResolutionScale12": "True"
}
```
### Move Pre-Render Phase
:::content-center
[!badge variant="success" text="~25% Performance Boost"] [!badge variant="danger" text="Please read the explanation below before applying"]
:::
==- :icon-question: View Full Documentation 
> [!IMPORTANT]  
> This FastFlag moves the Pre-Render task to an off thread after all other tasks are completed. By default, Pre-Render runs first, forcing the render thread to wait until the Pre-Render process finishes before it can start rendering a frame.

> [!NOTE]
> With this FastFlag enabled, Pre-Renderer is executed while the main thread is processing the previous frame. This adjustment allows the main thread to proceed without waiting for Pre-Renderer, leading to increased framerates at the expense of some frame latency.

> [!TIP]
> This flag is most effective in CPU-bound scenarios.

> [!CAUTION]
> Enabling this FastFlag may lead to input lag & crashes
===
```json
{
    "FFlagMovePrerender": "True"
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
### Enable Highlight Outlines on any Rendering API
```json
{
    "FFlagHighlightOutlinesOnMobile": "True"
}
```
### No Bloom/Clouds
@burgerboxer
```json
{
    "FFlagRenderNoLowFrmBloom": "False"
}
```
### Render Occlusion Culling
[@CloneTrooper1019](https://x.com/MaximumADHD/status/1832331711486865769)
```json
{
    "DFFlagUseVisBugChecks": "True",
    "FFlagEnableVisBugChecks27": "True",
    "FFlagVisBugChecksThreadYield": "True",
    "FIntEnableVisBugChecksHundredthPercent27": "100"
}
```
### Increased Particles on low graphics
@teeenoob
```json
{
    "FFlagDebugDeterministicParticles" : "True"
}
```
### Makes stuff slightly brighter
```json
{
    "FFlagRenderFixFog": "True"
}
```
### HyperThreading
```json
{
    "FFlagDebugCheckRenderThreading": "True",
    "FFlagRenderDebugCheckThreading2": "True"
}
```
### Maximum Threads
```json
{
    "FIntRuntimeMaxNumOfThreads": "2400"
}
```
### Minimum Threads
```json
{
    "FIntTaskSchedulerThreadMin": "3"
}
```
### Smoother Terrain
```json
{
    "FFlagDebugRenderingSetDeterministic": "True"
}
```
### Force Graphics Quality Level
```json
{
    "FIntRomarkStartWithGraphicQualityLevel": "1"
}
```
### Disable Player Shadows
```json
{
    "FIntRenderShadowIntensity": "0"
}
```
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
### Low Render Distance
```json
{
    "DFIntDebugRestrictGCDistance": "1"
}
```
### Limits light updates
```json
{
    "FIntRenderLocalLightUpdatesMax": "8",
    "FIntRenderLocalLightUpdatesMin": "6"
}
```
### Disables fade in and fade out animation every light update
```json
{
    "FIntRenderLocalLightFadeInMs": "0"
}
```
### Makes avatars shiny
==- :icon-question: View Documentation 
> [!TIP]
> **Everything goes black on below <3**

> [!NOTE]
> **DFIntDebugFRMQualityLevelOverride is there to set your graphics to 3 bars**

> [!TIP]
> **You can change it to anything above 3**
===
```json
{
    "DFIntRenderClampRoughnessMax": "-640000000",
    "DFIntDebugFRMQualityLevelOverride": "6"
}
```
### Disable PostFX
```json
{
    "FFlagDisablePostFx": "True"
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
### White Sky
@kezcn
> [!IMPORTANT]
> **Only applies to games with the default skybox**
```json
{
    "FFlagDebugSkyGray": "True",
    "FFlagSkyUseRGBEEncoding": "True"
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
### Lighting Attenuation
```json
{
    "FFlagNewLightAttenuation": "True"
}
```
### Enable GPULightCulling
> [!TIP]
> **Combine with [Lighting Attenuation](https://FastFlags/FastFlags-Collective/?tab=readme-ov-file#lighting-attenuation) for better vision**
```json
{
    "FFlagFastGPULightCulling3": "True"
}
```
### Enable CPULightCulling
```json
{
    "FFlagDebugForceFSMCPULightCulling": "True"
}
```
### Frame Buffer
> [!TIP]
> **0 makes white screen 1-3 makes other players have laggy movement, 4 is stable has better performance than 10 and less input lag**
```json
{
    "DFIntMaxFrameBufferSize": "4"
}
```
### Average Frame Delay
```json
{
    "DFIntMaxAverageFrameDelayExceedFactor": "3"
}
```
### Average Frame Delay + Frame Buffer
```json
{
    "DFIntMaxFrameBufferSize": "1",
    "FIntInterpolationAwareTargetTimeLerpHundredth": "100",
    "DFIntMaxAverageFrameDelayExceedFactor": "0"
}
```
### Low Quallity Terrain Textures
> [!TIP]
> **4 for less quality 16, 32, 64 for higher quality**
```json
{
    "FIntTerrainArraySliceSize": "4"
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
### Lower Quality Textures
```json
{
    "DFIntPerformanceControlTextureQualityBestUtility": "-1"
}
```
### No avatar textures
```json
{
    "DFIntTextureCompositorActiveJobs": "0"
}
```
### Texture Manager
> [!TIP]
> 1-4 Blurry, 5-7 low quality also removes studs, 8 Removes almost everything
```json
{
    "FIntDebugTextureManagerSkipMips": "8"
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
### ShadowMap Bias 
> [!IMPORTANT]
> **Future & ShadowMap only**
```json
{
    "FIntRenderShadowmapBias": "75"
}
```
### Limits number of animations being played
> [!TIP]
> **0 removes most player animations, 1-5 removes the walk animation after jumping**
```json
{
    "DFIntMaxActiveAnimationTracks": "0"
}
```
