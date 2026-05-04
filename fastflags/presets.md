<div align="center">

:icon-codescan-checkmark: Please read each line before importing

</div>

### :icon-sparkles-fill: High Quality
```json
{
    // === Vulkan Render API ===
    "FFlagDebugGraphicsDisableDirect3D11": "False", // Set to True to Disable DirectX
    "FFlagDebugGraphicsPreferVulkan": "False", // Set to True to use Vulkan

    // === Lighting ===
    "FFlagDebugForceFutureIsBrightPhase3": "True", // Enable Future Lighting

    // === Graphics ===
    "DFIntDebugFRMQualityLevelOverride": "21", // Force to max quality level
    "FFlagFastGPULightCulling3": "True", // Enable GPU Light Culling
    "DFIntMaxFrameBufferSize": "4", // Frame Buffer Size
    "DFFlagTextureQualityOverrideEnabled": "True", // Enable Texture Quality Override
    "DFIntTextureQualityOverride": "3", // Texture Quality Level
    "FIntDebugForceMSAASamples": "4", // Force MSAA (4x)

    // === UI ===
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000", // Disable Fullscreen Title Bar
    "FFlagUserShowGuiHideToggles": "True", // Optional UI Toggles

    // === Useful ===
    "FIntCameraMaxZoomDistance": "9999", // Doesn't work on all games
    "FFlagVoiceBetaBadge": "False", // Disable stupid badge
    "FFlagTopBarUseNewBadge": "False",
    "FFlagBetaBadgeLearnMoreLinkFormview": "False",
    "FFlagControlBetaBadgeWithGuac": "False",
    "FStringVoiceBetaBadgeLearnMoreLink": "null",
    "FFlagDebugEnableNewWebView2DevTool": "True", // Enable DevTools on WebViews

    // === Ads ===
    "FFlagAdServiceEnabled": "False", // Disable Ads

    // === Network ===
    "DFIntConnectionMTUSize": "1472", // MTU Size

    // === Loading ===
    "FFlagEnableQuickGameLaunch": "True", // Enable Quick Game Launch
    "DFIntNumAssetsMaxToPreload": "9999999", // Max asset preload
    "DFIntAssetPreloading": "9999999",

    // === Performance ===
    "FFlagDebugCheckRenderThreading": "True",
    "FFlagRenderDebugCheckThreading2": "True", // Enable HyperThreading
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False", // Remove 240 FPS Limit
    "DFIntTaskSchedulerTargetFps": "9999", // Set custom FPS target

    // === Telemetry ===
    "DFStringTelemetryV2Url": "0.0.0.0",
    "FFlagEnableTelemetryProtocol": "False",
    "FFlagEnableTelemetryService1": "False",
    "FFlagPropertiesEnableTelemetry": "False",
    "FFlagOpenTelemetryEnabled2": "False"
}
```

### :icon-rocket: Low Quality
```json
{
    // === Render API ===
    "FFlagDebugGraphicsPreferD3D11FL10": "True", // Use DirectX 10
    "FFlagHighlightOutlinesOnMobile": "True", // Allows Highlights to be used on DirectX 10

    // === Vulkan Render API (Set FFlagDebugGraphicsPreferD3D11FL10 to False if you want to use this) ===
    "FFlagDebugGraphicsDisableDirect3D11": "False", // Set to True to Disable DirectX
    "FFlagDebugGraphicsPreferVulkan": "False", // Set to True to use Vulkan

    // === Graphics ===
    "FIntRenderShadowIntensity": "0", // Remove Shadows
    "FIntGrassMovementReducedMotionFactor": "0", // Remove Grass
    "FIntFRMMinGrassDistance": "0", // Remove Grass
    "FIntFRMMaxGrassDistance": "0",
    "FIntRenderGrassDetailStrands": "0",
    "FFlagRenderNoLowFrmBloom": "True", // No Bloom/Clouds
    "FFlagDisablePostFx": "True", // Disable Post Processing Effects
    "FFlagDebugSkyGray": "True", // Gray Sky (optional)
    "DFIntCSGLevelOfDetailSwitchingDistance": "85", // Level of Detail Distance (Adjust to your liking)
    "DFIntCSGLevelOfDetailSwitchingDistanceL12": "85",
    "DFIntCSGLevelOfDetailSwitchingDistanceL23": "85",
    "DFIntCSGLevelOfDetailSwitchingDistanceL34": "85",
    "DFFlagTextureQualityOverrideEnabled": "True", // Force Texture Quality
    "DFIntTextureQualityOverride": "3",
    "DFIntDebugFRMQualityLevelOverride": "1", // Override FRM (Quality Level)
    "FFlagUserHideCharacterParticlesInFirstPerson": "True", // Hide 1st-person particles
    "FFlagFastGPULightCulling3": "True", // Enable GPU Light Culling
    "FIntRenderLocalLightUpdatesMax": "8", // Limit light updates
    "FIntRenderLocalLightUpdatesMin": "6",
    "FIntRenderLocalLightFadeInMs": "0", // Disable light fade animations

    // === UI ===
    "FFlagUserShowGuiHideToggles": "True", // Optional UI Toggles
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000", // Disable Fullscreen Title Bar
    "FIntRobloxGuiBlurIntensity": "0", // Remove Disconnect/Loading Blur

    // === Useful ===
    "FIntCameraMaxZoomDistance": "9999", // Doesn't work on all games
    "FFlagVoiceBetaBadge": "False", // Disable stupid badge
    "FFlagTopBarUseNewBadge": "False",
    "FFlagBetaBadgeLearnMoreLinkFormview": "False",
    "FFlagControlBetaBadgeWithGuac": "False",
    "FStringVoiceBetaBadgeLearnMoreLink": "null",
    "FFlagDebugEnableNewWebView2DevTool": "True", // Enable DevTools on WebViews

    // === Ads ===
    "FFlagAdServiceEnabled": "False", // Disable Ads

    // === Network ===
    "DFIntConnectionMTUSize": "1472", // MTU Size

    // === Loading ===
    "FFlagEnableQuickGameLaunch": "True", // Quick Game Launch
    "DFIntNumAssetsMaxToPreload": "9999999", // Increase Asset Preload Count
    "DFIntAssetPreloading": "9999999",

    // === Performance ===
    "FFlagDebugCheckRenderThreading": "True", // Enable HyperThreading
    "FFlagRenderDebugCheckThreading2": "True",
    "DFFlagDisableDPIScale": "True", // Disable DPI Scaling
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False", // Remove 240 FPS Limit
    "DFIntTaskSchedulerTargetFps": "9999",
    "FFlagMovePrerenderV2": "True", // PreRender (Remove if input lag occurs)
    "DFIntMaxFrameBufferSize": "4", // Frame Buffer

    // === Telemetry ===
    "DFStringTelemetryV2Url": "0.0.0.0",
    "FFlagEnableTelemetryProtocol": "False",
    "FFlagEnableTelemetryService1": "False",
    "FFlagPropertiesEnableTelemetry": "False",
    "FFlagOpenTelemetryEnabled2": "False"
}
```
