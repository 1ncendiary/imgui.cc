### DO NOT DISTURB/Disable Notifications
```json
{
    "FFlagToastNotificationsProtocolEnabled2": "False"
}
```
### Disable VC
> [!NOTE]
> Setting this to `True` will not do change anything
```json
{
    "DFFlagVoiceChat4": "False"
}
```
### Disable VC
> [!NOTE]
> Setting this to `True` will not do change anything
```json
{
    "DFFlagAvatarChatServiceEnableVoiceEnabledV1": "False"
}
```
### Removes translated supported message on join
> [!NOTE]
> `"Roblox automatically translates supported languages in chat."`
```json
{
    "FFlagChatTranslationEnableSystemMessage": "False"
}
```
### Allows you to customize which languages are available for the chat translation feature
> [!IMPORTANT]
> English cannot be removed.

@thefrenchguy4
```json
{
    "FStringChatTranslationEnabledLocales": "es_es,fr_fr,pt_br,de_de,it_it,ja_jp,ko_kr,id_id,tr_tr,zh_cn,zh_tw,th_th,pl_pl,vi_vn,ru_ru,"
}
```
### Remove long recommended section in homepage
```json
{
    "FIntGameGridFlexFeedItemTileNumPerFeed": "0"
}
```
### Disable Captures Keybind
```json
{
    "FFlagEnableCapturesHotkeyExperiment_v4": "False"
}
```
### Reduced Avatar Item Particle in FP
```json
{
    "FFlagUserHideCharacterParticlesInFirstPerson": "True"
}
```
### FPS Unlocker in Roblox Menu Settings
```json
{
    "FFlagGameBasicSettingsFramerateCap5": "True",
    "DFIntTaskSchedulerTargetFps": "0"
}
```
### Unlimited FPS Unlocker
```json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
    "DFIntTaskSchedulerTargetFps": "9999"
}
```
### GUI Hiding Toggles
```json
{
    "FFlagUserShowGuiHideToggles": "True",
    "GuiHidingApiSupport2": "True"
}
```
### Hide guis
> [!IMPORTANT]
> **Replace "ID" with any group ID that you are in.**

| Key combination   | Action                                                                    |
| ----------------- | ------------------------------------------------------------------------- |
| Ctrl + Shift + B  | Toggles GUIs in 3D space (BillboardGuis, SurfaceGuis, etc)                |
| Ctrl + Shift + C  | Toggles game-defined ScreenGuis                                           |
| Ctrl + Shift + G  | Toggles Roblox CoreGuis                                                   |
| Ctrl + Shift + N  | Toggles player names, and other BillboardGuis that show up above a player |
```json
{
    "DFIntCanHideGuiGroupId": "ID"
}
```
### Remove layared clothing related for searching in lua app catalog
```json
{
    "FStringAXCategories": "ClassicShirts.ClassicTShirts.ClassicPants"
}
```
### Disable Fullscreen Title Bar
```json
{
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000"
}
```
### Stuttery Animation Fix
```json
{
    "DFIntTimestepArbiterThresholdCFLThou": "300"
}
```
### Disable In-game Advertisements
```json
{
    "FFlagAdServiceEnabled": "False"
}
```
### Disable Telemetry 
```json
{
    "DFStringTelemetryV2Url": "0.0.0.0",
    "FFlagEnableTelemetryProtocol": "False",
    "FFlagEnableTelemetryService1": "False",
    "FFlagPropertiesEnableTelemetry": "False",
    "FFlagOpenTelemetryEnabled2": "False"
}
```
### Surf the web inside of Roblox
> [!IMPORTANT]
> **Click the Beta badge or the 13+ badge to open the webview browser.**
```json
{
    "FFlagTopBarUseNewBadge": "True",
    "FStringTopBarBadgeLearnMoreLink": "https://google.com/",
    "FStringVoiceBetaBadgeLearnMoreLink": "https://google.com/"
}
```
### MTU
==- :icon-question: View Full Documentation
> [!TIP]
> **Identify the Current MTU**
> - **Windows**: Open Command Prompt and type `netsh interface ipv4 show subinterfaces`.
> - **Linux**: Use `ifconfig` or `ip link show` to find the current MTU of your network interface.

> [!TIP]
> **Determine the Optimal MTU**
> - **Ping Test**: Use the `ping` command with the `-f` flag (to avoid fragmentation) and the `-l` (or `-s` on Linux) flag to set the packet size.
> - **Example for Windows**:
>   ```bash
>   ping roblox.com -f -l 1472
>   ```
> - **Example for Linux**:
>   ```bash
>   ping -s 1472 -M do roblox.com
>   ```
> - Start with a packet size of 1472 bytes, then reduce by 10-12 bytes if needed until you find the largest size that doesn't fragment. Add 28 bytes to this number to get the optimal MTU.
===
```json
{
    "DFIntConnectionMTUSize": "MTU_HERE"
}
```
### No Internet Disconnect 
> [!NOTE]
> **You will still be kicked but the message wont show.**
```json
{
    "DFFlagDebugDisableTimeoutDisconnect": "True"
}
```
### Adjust Default Timeout Time
> [!TIP]
> **1 second = 1000**

@dis_spencer
```json
{
    "DFIntDefaultTimeoutTimeMs": "10000"
}
```
### Quick Game Launch 
> [!CAUTION]
> **This can cause some bugs**
```json
{
    "FFlagEnableQuickGameLaunch": "True"
}
```
### Increased Asset Preloading Count
==- :icon-question: View Full Documentation
> [!NOTE]
> **Increasing the maximum limit of preloaded assets from 100 to infinite allows games you've already played to load much faster by instantly accessing previously loaded assets.**

> [!IMPORTANT]
> **For this to be effective, the game must have been fully loaded at least once, preferably with the entire map cached.**

> [!TIP]
> **If a game has a "Skip Loading" button, it's recommended to use it. These games typically include a countdown timer that, after reaching zero, merely confirms that all assets are loaded.**
===
@spectroscopic
```json
{
    "DFIntNumAssetsMaxToPreload": "9999999",
    "DFIntAssetPreloading": "9999999"
}
```
### Disable In-Game Purchases
```json
{
    "DFFlagOrder66": "True"
}
```
### Disable Chat
```json
{
    "FFlagDebugForceChatDisabled": "True"
}
```
### Disable Dynamic Heads Animations
```json
{
    "DFIntAnimationLodFacsDistanceMin": "0",
    "DFIntAnimationLodFacsDistanceMax": "0",
    "DFIntAnimationLodFacsVisibilityDenominator": "0"
}
```
### Automatically unmutes your mic on join (VC)
```json
{
    "FFlagDebugDefaultChannelStartMuted": "False"
}
```
### opt-out Experience Language
> [!NOTE]
> **Removes the Experience Language option in settings**
```json
{
    "FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0"
}
```
### Lets you change the zoom out limit
> [!IMPORTANT]
> **Only applies to games that has not changed the default zoom limit**
```json
{
    "FIntCameraMaxZoomDistance": "9999"
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
### Change Age Rating Learn More Link
```json
{
    "FStringExperienceGuidelinesExplainedPageUrl": "https://playboicarti.com"
}
```
### Rename Party 2 Roblox Chat
```json
{
    "FFlagAppChatRebrandStringUpdates": "False"
}
```
