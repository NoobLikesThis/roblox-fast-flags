# roblox-fflags
### [fflag tracker](https://raw.githubusercontent.com/MaximumADHD/Roblox-Client-Tracker/roblox/FVariables.txt)
## LINKS
### [FLEASION 1 (TOP TIER #1)](https://fleasion.github.io/)
### [FLEASION 2 (TOP TIER #1) (alternative)](https://github.com/fleasion/Fleasion/releases)
### ------------------------
### [fishstrap 1](https://fishstrap.app/)
### [fishstrap 2 (alternative)](https://github.com/returnrqt/bloxstrap/)
### [bloxstrap 1](https://bloxstraplabs.com/)
### [bloxstrap 2 (alternative)](https://github.com/bloxstraplabs/bloxstrap)
### [froststrap 1](https://github.com/Froststrap/Froststrap)
### [froststrap 2 (alternative)](https://froststrap.github.io/)
## GOTO
[Physics](#physics)

[Untested](#untested)

[the idk section](#random)
## physics
### freeze clientsided
###### ctrl +f7
``` json
{
  "DFFlagDebugEnableInterpThrottle": true
}
```
### speed
###### This makes you fast in games like Counter-Strike 
```json
{
  "DFIntRaycastMaxDistance": "0",
  "DFFlagDebugHumanoidNewPhysicsEnabled": True
}
```
### This Fast Flags Makes Player Spin Only Works On Some Games Like Combat Warriors if You Changed The DFIntRaycastMaxDistance Value To 1 It's Gonna Make Weird Glitchs

Game Link: https://www.roblox.com/games/4282985734/Combat-Warriors

Fast Flags:
```json
{
  "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "-1",
  "DFFlagDebugHumanoidNewPhysicsEnabled": "true"
}
```
### keep falling
It makes the player keep falling, and you have to jump to get back up.

Video: https://www.youtube.com/watch?v=yzDR3ZQ85Uw
```json
{
  "DFIntRaycastMaxDistance": "1",
  "DFFlagDebugHumanoidNewPhysicsEnabled": true
}
```
### It makes things fly when you jump on them

Fast Flags:
```json
{
  "DFFlagDebugHumanoidNewPhysicsEnabled": true,
  "DFIntSolidFloorPercentForceApplication": "-10000",
  "DFIntNonSolidFloorPercentForceApplication": "-10000"
}
```
### ESP
```json
{
  "DFFlagDebugDrawBroadPhaseAABBs": "True",
  "FIntCameraFarZPlane": "0"
}
```
### more hitboxes
###### used to do mesh noclip.
``` json
{
    "DFIntPhysicsDecompForceUpgradeVersion": "1500"
}
```
### Stick unanchored parts to you
##### - = up, + = down
###### flings you a bit
``` json
{
    "DFIntSolidFloorPercentForceApplication": "-1000",
    "DFIntNonSolidFloorPercentForceApplication": "-5000"
}
```
### slide on wall walks/hops
###### buggy. only works in a certain angle.
``` json
{
    "DFIntMaximumFreefallMoveTimeInTenths": "2147483648"
}
```
### Tool Desyncs
``` json
    {
        "DFIntSimBlockLargeLocalToolWeldManipulationsThreshold": "-1"
    }
```
### Invisible 1

> \[!NOTE\] **Restricts the client from sending any physics-related
> information. This means other people can topple you over.**

``` json
{
    "DFIntPhysicsSenderMaxBandwidthBps": "1",
    "DFIntPhysicsSenderMaxBandwidthBpsScaling": "0"
}
```
### Invisible 2

> \[!NOTE\] **Locks your character's position on the server to (0, 0,
> 0), having the side effect of turning you invisible. This only affects
> the server and other clients, not you. server-sided things that rely
> on your position, like clicking to get tools, will not function. In
> some games these can be abusable. Here is a list of them:
> [Link](https://github.com/luafv/rbxflags/blob/master/assets/lists/experiences/specific.md)**

``` json
{
    "DFIntGameNetPVHeaderTranslationZeroCutoffExponent": "10"
}
```
### Physics test
#### This fast flag sets the current physics "FPS", this slows down all the physics related stuff aka falling, walking. Change 1, 2, 3 and 4 for an effect, use 3 and with 60 fps for the best effect, use 4 with any fps lower than 45.
##### values like 1000 make it so  u cant tab glitch.

``` json
{
  "DFIntMaxMissedWorldStepsRemembered": "1"
}
```
##### Games: any game (obbys are easier to do with slow Physics)

### warp
##### to warp, first walk and continue walking then hold the white window bar and untab.
``` json
{
    "DFIntMaxMissedWorldStepsRemembered": "1000"
}
```
### wallglide
``` json
{
"DFIntMaximumUnstickForceInGs": "-4"
}
```
## untested
### Remap R6 to R15 Rigs/Weird Movement
```json
{
    "FFlagRemapAnimationR6ToR15Rig": "True"
}
```
### Network Ownership
###### better [network ownership](https://create.roblox.com/docs/physics/network-ownership) of parts
``` json
    {
        "DFIntMinClientSimulationRadius": "2147000000",
        "DFIntMinimalSimRadiusBuffer": "2147000000",
        "DFIntMaxClientSimulationRadius": "2147000000"
    }
```
### fixed network ownership
``` json
{
    "DFIntMinClientSimulationRadius": "2147000000",
    "DFIntMinimalSimRadiusBuffer": "2147000000",
    "DFIntMaxClientSimulationRadius": "2147000000",
    "DFFlagDebugPhysicsSenderDoesNotShrinkSimRadius": "True",
    "FFlagDebugUseCustomSimRadius": "True"
}
```

### Drunk
``` json
    {
        "FFlagSimAdaptiveTimesteppingDefault2": "True",
        "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
        "DFFlagSimHumanoidTimestepModelUpdate": "True"
    }
```
### Weird Leg Movement
###### patched roughly in 2025 :c
``` json

    {
        "DFFlagAnimatorPostProcessIK": "True"
    }
```
### No Animations
###### Stops the game from trying to replicate your animations in the server. You dont have animations in the server but you do for your client
``` json
{
    "DFIntReplicatorAnimationTrackLimitPerAnimator": "-1"
}
```
### Disable other players animations (Clientsided)
``` json
{
  "FFlagProcessAnimationLooped":"False",
  "FFlagReplicateAnimationLooped":"False"
}
```
### Limits number of animations being played
##### 0 removes most player animations, 1-5 removes the walk animation after jumping
``` json
{
    "DFIntMaxActiveAnimationTracks": "0"
}
```
### spin 2
###### depends on walkspeed
``` json
{
 "FFlagSimAdaptiveTimesteppingDefault2": "True",
 "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
 "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### spinny test
###### uses debounce instead.
``` json
{
    "DFIntSimTimestepMultiplierDebounceCount": "-1100000",
    "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999"
}
```


### Drive vehicles slowly
###### set to -1 for slowest, this fflag changes the physicsreal throttle (see physicsreal by pressing shift + f4
###### @tyetonix
```json
{
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "0"
}
```
### Slide on Terrain/Meshes
##### @tyetonix
``` json
{
    "DFIntSmoothTerrainPhysicsRayAabbSlop": "-9999"
}
```
### improved
``` json
{
    "DFIntSmoothTerrainPhysicsRayAabbSlop": "-9999",
    "DFIntMaximumFreefallMoveTimeInTenths": "2147483648"
}
```
# random
### faster preloading
``` json
{
    "DFIntAssetPreloading": "9999999"
}
```
### MTU 
###### 1472 good
```json
{
    "DFIntConnectionMTUSize": "MTU_HERE"
}
```
### Preserve rendering quality with display setting
```json
{
    "DFFlagDisableDPIScale": "True"
}
```
### reduce avatar item particles in first person
``` json
{
    "FFlagUserHideCharacterParticlesInFirstPerson": "True"
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
### Disable voicechat
###### Setting this to True will not do anything 
###### [TIP] Use PlaceFilter for specific games
```json
{
    "DFFlagVoiceChat4": "False"
}
```
### Disable Dynamic Heads Animations
###### https://roblox.fandom.com/wiki/Dynamic_Head
```json
{
    "DFIntAnimationLodFacsDistanceMin": "0",
    "DFIntAnimationLodFacsDistanceMax": "0",
    "DFIntAnimationLodFacsVisibilityDenominator": "0"
}
```
### opt-out Experience Language
###### Removes the Experience Language option in settings
```json
{
    "FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0"
}
```
### Exclusive Fullscreen
```json
{
    "FFlagHandleAltEnterFullscreenManually": "False"
}
```
### quick game launch
###### may cause bugs
``` json
{
    "FFlagEnableQuickGameLaunch": "True"
}
```
### remove fullscreen title bar
``` json
{
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000"
}
```
### force MSAA
###### values are 0, 1, 2, 4 and 8. values over 4 may cause viewport bugs
``` json
{
    "FIntDebugForceMSAASamples": "4"
}
```
### new camera mode
FFlagNewCameraControls
FFlagNewCameraControls_AltDisableZoom
FFlagNewCameraControls_DisableMMBFocus
FFlagNewCameraControls_IncrementalZoom
FFlagNewCameraControls_PlanarPan
FFlagNewCameraControls_SeparateRotateShift
FFlagNewCameraControls_SmoothingSetting
FFlagNewCameraControlsBetaFeature
``` json
{
    "FFlagNewCameraControls": "True"
}
```
### Always display Render Stats
###### pretty self explanatory fflag, you can't disable them using the hotkey
```json
{
    "FFlagDebugAlwaysDisplayRenderStats": "true"
}
```
### New Report Menu
```json
{
    "FStringSelectInSceneReportMenuOverrideUserIds": "UserID"
}
```
### remove unnecessary kicks
###### removes being kicked for being afk
``` json
{
    "DFFlagDebugDisableTimeoutDisconnect": "True"
}
```
### Chrome UI TopBar
``` json
{
    "FFlagEnableInGameMenuChrome": "True"
}
```
### red font
###### might not work idk
```json
{
    "FStringDebugHighlightSpecificFont": "rbxasset://fonts/families/BuilderSans.json"
}
```
### V2 Menu
###### enables the 2020 sidebar menu
```json
{
    "FIntNewInGameMenuPercentRollout3": "100",
}
```
### Enable Highlight Outlines on any Rendering API
``` json
{
    "FFlagHighlightOutlinesOnMobile": "True"
}
```
### Break Collectible Icon
``` json
{
    "FFlagDisplayCollectiblesIcon": "False"
}
```
### Break Top Bar Menu
``` json
{
    "FStringNewInGameMenuForcedUserIds": "UserID",
    "FFlagEnableInGameMenuChrome": "True"
}
```
### Dont Render Screen GUIs
``` json
{
    "FFlagDebugDontRenderScreenGui": "True"
}
```
### Overlay that shows what you type
``` json
{
    "FFlagDebugTextBoxServiceShowOverlay": "True"
}
```
### Hides gui
``` json
{
    "FFlagDebugAdornsDisabled":  "True"
}
```
### Disable Bubble Chat
``` json
{
    "FFlagEnableBubbleChatFromChatService": "False"
}
```
### Disable In-Game Purchases
##### gives an error when you try and buy something.
``` json
{
    "DFFlagOrder66": "True"
}
```
### Better shadows
##### Loading will take longer but the shadows are much better
``` json
{
    "FFlagRenderInitShadowmaps": "true"
}
```
### Raycast Performance Improvements
##### tip: Uses workspace:Raycast() instead of worldmodel:FindPartOnRayWithIgnoreList()
``` json
{
    "FFlagUserRaycastPerformanceImprovements": "true"
}
```
### Render Occlusion Culling
##### [@CloneTrooper1019](https://x.com/MaximumADHD/status/1832331711486865769)
``` json
{
    "DFFlagUseVisBugChecks": "True"
}
```
### Remove Unrequired Connections
##### Disconnects unrequired connections, better memory usage
``` json
{
    "FFlagUserUpdateInputConnections": "true"
}
```
### texture override
```json
{
    "DFFlagTextureQualityOverrideEnabled": "True",
    "DFIntTextureQualityOverride": "3"
}
```
### Smoother/Faster Input
##### Tip: When enabled the game will use an updated implementation for processing user input, which may lead to smoother and more responsive interactions. This flag controls the refactoring of the legacy input handling system in Roblox.
##### Recommendation: Test your game thoroughly after enabling this flag to ensure that everything functions as expected.
``` json
{
    "FFlagLuaAppLegacyInputSettingRefactor": true
}
```
### Move Pre-Render Phase [~25% Performance Boost]
###### This FastFlag moves the Pre-Render task to an off thread after all other tasks are completed. By default, Pre-Render runs first, forcing the render thread to wait until the Pre-Render process finishes before it can start rendering a frame.
###### With this FastFlag enabled, Pre-Renderer is executed while the main thread is processing the previous frame. This adjustment allows the main thread to proceed without waiting for Pre-Renderer, leading to increased framerates at the expense of some frame latency.
###### This flag is most effective in CPU-bound scenarios.
###### This fflag might cause issues
###### @blobanium
```json
{
    "FFlagMovePrerender": "True",
    "FFlagMovePrerenderV2": "true"
}
```
## untest_shader
### semi fullbright
``` json
{
    "FFlagFastGPULightCulling3": "True",
    "FIntRenderShadowIntensity": "0",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "FFlagNewLightAttenuation": "True",
    "FIntRenderShadowmapBias": "-1",
    "DFFlagDebugPauseVoxelizer": "True"
}
```
### fullbright 1
###### use in games with massive or games with lots of clouds, make sure the game is daytime or has daytime.
###### fullbright 1 and 2 will let you noclip a bit inside a wall, be-aware.
###### tip: change the DFIntDebugFRMQualityLevelOverride fflag to 0 when you dont want quality 1 and wanna change it in game, best to hide ur fullbright while someone is watching.
``` json
{
    "FFlagFastGPULightCulling3": "True",
    "FIntRenderShadowIntensity": "0",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "FFlagNewLightAttenuation": "True",
    "FIntRenderShadowmapBias": "-1",
    "DFFlagDebugPauseVoxelizer": "True",
    "DFIntDebugFRMQualityLevelOverride": "1",
    "DFFlagDebugRenderForceTechnologyVoxel": "True",
    "FFlagRenderFixFog": "True",
    "FFlagDisablePostFx": "True"
}
```
### fullbright 2
###### use in games with massive or games with lots of clouds, make sure the game is daytime or has daytime.
###### same stuff needed as fullbright but its better, fullbright 1 and 2 will let you noclip a bit inside a wall, be-aware.
##### tip: change the DFIntDebugFRMQualityLevelOverride fflag to 0 when you dont want quality 1 and wanna change it in game, best to hide ur fullbright while someone is watching.
##### tip: for expirenced people, add opengl and remove ur old rendering mode, remove the shaders with a fflag for less shadows.
##### fflags in fflags folder, random fflags 2.

``` json
{
    "FFlagFastGPULightCulling3": "True",
    "FIntRenderShadowmapBias": "-1",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "FIntRenderShadowIntensity": "0",
    "FFlagRenderFixFog": "True",
    "DFFlagDebugRenderForceTechnologyVoxel": "True",
    "FFlagRenderNoLowFrmBloom": "false",
    "DFIntDebugFRMQualityLevelOverride": "1",
    "FIntBloomFrmCutoff": "1654515",
    "DFFlagDebugPauseVoxelizer": "True",
    "FFlagNewLightAttenuation": "True",
    "FFlagFRMRefactor": "false",
    "FFlagDisablePostFx": "True"
}
```
## Visuals ig
### white everything
###### by [new guy](https://github.com/Storm99999)
``` json
  "FFlagSkyUseRGBEEncoding": "True",
```
### white sky
###### by [new guy](https://github.com/Storm99999)
``` json
  "FFlagSkyUseRGBEEncoding": "True",
  "FFlagDebugSkyGray": "True",
```
### grey sky
##### i thought that you guys wanted it
``` json
{
    "FFlagDebugSkyGray": "True",
}
```
### black sky
##### buggy.
###### i def dont have to put credits
``` json
{
    "FFlagDebugSkyGray": true,
    "FIntCameraFarZPlane": 600
}
```
### colorful sky
``` json
{
    "DFFlagTextureQualityOverrideEnabled": "True",
    "DFIntTextureQualityOverride": "0",
    "FFlagHandleAltEnterFullscreenManually": "False",
    "FFlagDebugGraphicsPreferVulkan": "True",
    "FIntDebugFRMOptionalMSAALevelOverride": "0",
    "FIntVertexSmoothingGroupTolerance": "0",
    "FIntDebugTextureManagerSkipMips": "8",
    "FIntDebugForceMSAASamples": "0"
}
```
### texture skipmips
```json
{
    "FFlagRenderUseTextureManager224": "false",
    "FIntDebugTextureManagerSkipMips": "8"
}
```
### quality level override
###### use 1-21
``` json
{
    "DFIntDebugFRMQualityLevelOverride": "2"
}
```
### frm levels
```
Low

1 = 3
2 = 2
3 = 6

High

4 = 7
5 = 11
6 = 14
7 = 15 
8 = 17
9 = 18
10 = 21
```
### HyperThreading
``` json
{
    "FFlagDebugCheckRenderThreading": "True",
    "FFlagRenderDebugCheckThreading2": "True"
}
```
### Makes stuff slightly brighter
``` json
{
    "FFlagRenderFixFogSkyboxOrientation": "True"
}
```
### Applies cool colors to stuff
``` json
{
"FFlagDebugDisplayUnthemedInstances": "True"
}
```
### Enable GPULightCulling
###### use with lighting attenuation for better vision
``` json
{
    "FFlagFastGPULightCulling3": "True"
}
```
### Enable CPULightCulling
``` json
{
    "FFlagDebugForceFSMCPULightCulling": "True"
}
```
### Esp..?
###### adds red circle under avatar and a grey thing above
###### https://github.com/NoobLikesThis/using-older-fflags
``` json
{
    "FFlagDebugAvatarChatVisualization": "True",
    "FFlagEnableInGameMenuChromeABTest4": "False",
    "FFlagEnableInGameMenuChrome": "False",
    "FFlagEnableInGameMenuSongbirdABTest": "False"
}
```
### humanoid Outline
> [!NOTE]
> **Draws an outline around every part and every humanoid**
```json
{
    "DFFlagDebugDrawBroadPhaseAABBs": "True"
}
```
### fflag above but more complex
> [!NOTE]
> **Draws an outline around every body part**
```json
{
    "DFFlagDebugDrawBvhNodes": "True"
}
```
### make low quality roblox memes
``` json
{
  "DFIntDebugDynamicRenderKiloPixels":"2"
}
```
### Adds an UI in game, which highlights any part player touches (like ground, Meshes etc.). It's a non-functioning UI too. Also adds a blue circle to your humanoid.
```json
{
    "FFlagDebugHumanoidRendering": "True"
}
```
### Crash roblox 1 
##### when you try to launch roblox it won't open
```json
{
    "DFFlagDebugSimulateHangAtStartup": "True"
}
```
### Crash roblox 2
##### the same thing from above but it only crashes when you try to close roblox
```json
{
    "DFFlagDebugSimulateHangAtShutdown": "True"
}
```
### Shows the state of a flag
```json
{
    "FStringDebugShowFlagState": "FLAG_HERE"
}
```
> [!TIP]
> 
```json
{
    "FStringDebugShowFlagState": "DFIntTaskSchedulerTargetFps, ChannelName"
}
```
### Show Outlined Chunks
```json
{
    "FFlagDebugLightGridShowChunks": "True"
}
```
### Show Outlined Chunks that are being interacted
```json
{
    "DFFlagDebugEnableStreamingSolverVisualization": "True"
}
```
### Prevents Remote Events from running
###### @spectroscopic
```json
{
    "DFIntRemoteEventSingleInvocationSizeLimit": "1"
}
```
### log player joins,leaves,messages
###### only works with the new chat
###### @return_request
```json
{
    "FStringDebugLuaLogLevel": "trace",
    "FStringDebugLuaLogPattern": "ExpChat/mountClientApp"
}
```
### Max dev console log count
###### Control how many developer console logs can be shown at once, for example if you set the limit to be 100, then 100 different log messages will be shown while any older ones will be deleted when the limit is reached
###### @satlybpro
``` json
{
    "FIntNewDevConsoleMaxLogCount": "2147483647"
}
```
### Replace all Decals with a Test Image
###### @.rbx.bloxy
```json
{
    "FFlagDebugTestImageDrawItem": "True"
}
```
### Self Explanatory 1
```json
{
    "DFFlagDebugPrintDataPingBreakDown": "True"
}
```
### Self Explanatory 2
```json
{
    "DFFlagDebugAudioLogging": "True"
}
```
### Duplicate of Above
```json
{
    "DFFlagDebugAudioLogging2": "True"
}
```
### Self Explanatory 3
> [!NOTE]
> **Disable CTM Climbing**
```json
{
    "FFlagUserClickToMoveSupportAgentCanClimb2": "False"
}
```
### Self Explanatory 4
###### LDL dev console printing
###### @tyetonix
```json
{
    "DFFlagDebugSimLDLProgramPrintBuildStats": "True",
    "DFFlagDebugSimLDLProgramPrintExecStats": "True"
}
```
### Self Explanatory 5
###### prints body allocations counts in dev console
###### @tyetonix
```json
{
    "FFlagDebugCountSimBodyAllocations": "True"
}
```
### Abusive Game Specific Presets
### **EVERYTHING U SEE BELOW IS NOT TESTED**
### Low Graphics - High Render Distance
``` json
{
"DFFlagDebugRenderForceTechnologyVoxel": true,
"DFIntDebugFRMQualityLevelOverride": 1,
"FIntRenderShadowIntensity": 0
}
```

### Lower Ping
``` json
{
"DFIntConnectionMTUSize": 900,
"FIntRakNetResendBufferArrayLength": "128",
"FFlagOptimizeNetwork": "True",
"FFlagOptimizeNetworkRouting": "True",
"FFlagOptimizeNetworkTransport": "True",
"FFlagOptimizeServerTickRate": "True",
"DFIntServerPhysicsUpdateRate": "60",
"DFIntServerTickRate": "60",
"DFIntRakNetResendRttMultiple": "1",
"DFIntRaknetBandwidthPingSendEveryXSeconds": "1",
"DFIntOptimizePingThreshold": "50",
"DFIntPlayerNetworkUpdateQueueSize": "20",
"DFIntPlayerNetworkUpdateRate": "60",
"DFIntNetworkPrediction": "120",
"DFIntNetworkLatencyTolerance": "1",
"DFIntMinimalNetworkPrediction": "0.1"
}
```

### Boost FPS (Comfort To Play)
``` json
{
"DFIntCSGLevelOfDetailSwitchingDistance": 250,
"DFIntCSGLevelOfDetailSwitchingDistanceL12": 500,
"DFIntCSGLevelOfDetailSwitchingDistanceL23": 750,
"DFIntCSGLevelOfDetailSwitchingDistanceL34": 1000,
"DFIntTextureQualityOverride": 1,
"FFlagDisablePostFx": true
}
```

### OPTIMIZATION FFLAG
###### low quality mode
``` json
{
  "FFlagDebugGraphicsPreferD3D11FL10": "True",
  "FFlagGameBasicSettingsFramerateCap5": "False",
  "DFIntTaskSchedulerTargetFps": "5588562",
  "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
  "DFIntMaxFrameBufferSize": "4",
  "FIntDebugForceMSAASamples": "0",
  "DFFlagDebugPerfMode": "True",
  "FFlagDisablePostFx": "True",
  "FFlagFixGraphicsQuality": "True",
  "DFFlagDisableDPIScale": "True",
  "FFlagHandleAltEnterFullscreenManually": "False",
  "DFIntCSGLevelOfDetailSwitchingDistance": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0",
  "DFFlagDebugRenderForceTechnologyVoxel": "True",
  "DFFlagVoxelizerDisableTerrainSIMD": "True",
  "DFFlagDebugSkipMeshVoxelizer": "True",
  "FIntRenderShadowIntensity": "0",
  "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
  "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
  "FIntRenderLocalLightUpdatesMax": "1",
  "FIntRenderLocalLightUpdatesMin": "1",
  "FFlagDebugRenderingSetDeterministic": "True",
  "FIntTerrainArraySliceSize": "4",
  "FIntFRMMinGrassDistance": "0",
  "FIntFRMMaxGrassDistance": "0",
  "FIntRenderGrassDetailStrands": "0"
}
```
### OPTIMIZATION FFLAG
###### balanced quality mode.
``` json
{
  "FFlagDebugGraphicsPreferD3D11FL10": "True",
  "FFlagGameBasicSettingsFramerateCap5": "False",
  "DFIntTaskSchedulerTargetFps": "5588562",
  "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
  "DFIntMaxFrameBufferSize": "4",
  "FIntDebugForceMSAASamples": "0",
  "DFFlagDebugPerfMode": "True",
  "FFlagFixGraphicsQuality": "True",
  "DFFlagDisableDPIScale": "True",
  "FFlagHandleAltEnterFullscreenManually": "False",
  "DFFlagDebugRenderForceTechnologyVoxel": "True",
  "DFFlagVoxelizerDisableTerrainSIMD": "True",
  "DFFlagDebugSkipMeshVoxelizer": "True",
  "FIntRenderShadowIntensity": "0",
  "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
  "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
  "FIntRenderLocalLightUpdatesMax": "1",
  "FIntRenderLocalLightUpdatesMin": "1",
  "FFlagDebugRenderingSetDeterministic": "True",
  "FIntTerrainArraySliceSize": "8",
  "FIntFRMMinGrassDistance": "0",
  "FIntFRMMaxGrassDistance": "0",
  "FIntRenderGrassDetailStrands": "0"
}
```
### OPTIMIZATION FFLAG
###### high quality mode optimized.
``` json
{
  "FFlagDebugGraphicsPreferD3D11FL10": "True",
  "FFlagGameBasicSettingsFramerateCap5": "False",
  "DFIntTaskSchedulerTargetFps": "5588562",
  "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
  "DFIntMaxFrameBufferSize": "4",
  "FIntDebugForceMSAASamples": "0",
  "DFFlagDebugPerfMode": "True",
  "FFlagDisablePostFx": "True",
  "FFlagFixGraphicsQuality": "True",
  "DFFlagDisableDPIScale": "True",
  "FFlagHandleAltEnterFullscreenManually": "False",
  "DFFlagDebugRenderForceTechnologyVoxel": "True",
  "DFFlagVoxelizerDisableTerrainSIMD": "True",
  "DFFlagDebugSkipMeshVoxelizer": "True",
  "FIntRenderShadowIntensity": "0",
  "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
  "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
  "FIntRenderLocalLightUpdatesMax": "1",
  "FIntRenderLocalLightUpdatesMin": "1",
  "DFFlagTextureQualityOverrideEnabled": "True",
  "DFIntTextureQualityOverride": "3",
  "FFlagDebugRenderingSetDeterministic": "True",
  "FIntTerrainArraySliceSize": "12",
  "FIntFRMMinGrassDistance": "0",
  "FIntFRMMaxGrassDistance": "0",
  "FIntRenderGrassDetailStrands": "0"
}
```
### kaids optimization fflags
``` json
{
  "DFIntTaskSchedulerTargetFps": 540,
  "FFlagHandleAltEnterFullscreenManually": false,
  "FFlagFastGPULightCulling3": true,
  "FFlagPreloadAllFonts": true,
  "DFIntS2PhysicsSenderRate": 100,
  "FFlagFixGraphicsQuality": true,
  "FFlagAdServiceEnabled": false,
  "DFIntClientLightingTechnologyChangedTelemetryHundredthsPercent": 0,
  "DFStringCrashUploadToBacktraceBaseUrl": "null",
  "DFStringCrashUploadToBacktraceMacPlayerToken": "null",
  "DFStringCrashUploadToBacktraceWindowsPlayerToken": "null",
  "GoogleAnalyticsAccountPropertyID": "null",
  "GoogleAnalyticsAccountPropertyIDPlayer": "null",
  "FStringCoreScriptBacktraceErrorUploadToken": "null",
  "FStringGamesUrlPath": "/games/",
  "DFFlagClientBaseNetworkMetrics": false,
  "DFStringRobloxAnalyticsURL": "null",
  "DFStringTelegrafHTTPTransportUrl": "null",
  "DFStringAltTelegrafHTTPTransportUrl": "null",
  "DFStringTelegrafAddress": "127.0.0.1",
  "DFStringAltTelegrafAddress": "127.0.0.1",
  "DFStringTelemetryV2Url": "null",
  "DFFlagEnableLightstepReporting2": false,
  "DFIntLightstepHTTPTransportHundredthsPercent2": 0,
  "DFStringLightstepHTTPTransportUrlHost": "null",
  "DFStringLightstepHTTPTransportUrlPath": "null",
  "DFStringLightstepToken": "null",
  "FFlagDebugDisableTelemetryEphemeralCounter": true,
  "FFlagDebugDisableTelemetryEphemeralStat": true,
  "FFlagDebugDisableTelemetryEventIngest": true,
  "FFlagDebugDisableTelemetryPoint": true,
  "FFlagDebugDisableTelemetryV2Counter": true,
  "FFlagDebugDisableTelemetryV2Event": true,
  "FFlagDebugDisableTelemetryV2Stat": true,
  "DFStringHttpPointsReporterUrl": "null",
  "DFStringAltHttpPointsReporterUrl": "null",
  "DFStringAnalyticsEventStreamUrlEndpoint": "null"
}
```
### MY OPTIMIZATION FFLAG (CAN CRASH DUE TO VULKAN)
###### make sure to remove preferdirect3d11 and not disabledirect3d11 dont use in fighting games.
``` json
{
  "FLogNetwork": "7",
  "FFlagDisableNewIGMinDUA": "True",
  "FFlagEnableInGameMenuControls": "True",
  "FFlagEnableInGameMenuModernization": "True",
  "FFlagEnableMenuControlsABTest": "False",
  "FFlagEnableV3MenuABTest3": "False",
  "FFlagFixGraphicsQuality": "True",
  "FFlagEnableInGameMenuChrome": "False",
  "FFlagEnableInGameMenuChromeABTest3": "False",
  "DFIntTextureQualityOverride": "3",
  "DFFlagTextureQualityOverrideEnabled": "True",
  "FIntPGSPenetrationMarginMax": "-100000000",
  "FIntPGSPenetrationMarginMin": "-100000000",
  "FFlagDebugDisableTelemetryEphemeralStat": "True",
  "FFlagDebugDisableTelemetryEventIngest": "True",
  "FFlagDebugDisableTelemetryPoint": "True",
  "FFlagDebugDisableTelemetryV2Counter": "True",
  "FFlagDebugDisableTelemetryV2Event": "True",
  "FFlagDebugDisableTelemetryV2Stat": "True",
  "DFIntCSGLevelOfDetailSwitchingDistance": "500",
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": "1000",
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": "2000",
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": "4000",
  "FFlagDebugDisableTelemetryEphemeralCounter": "True",
  "FFlagDebugGraphicsDisableDirect3D11": "True",
  "FFlagDebugGraphicsPreferVulkan": "True",
  "DFFlagDebugRenderForceTechnologyVoxel": "True",
  "DFIntDebugFRMQualityLevelOverride": "2",
  "DFIntCanHideGuiGroupId": "32380007",
  "FIntRenderShadowIntensity": "0",
  "FFlagCoreGuiTypeSelfViewPresent": "False",
  "FFlagInGameMenuV1FullScreenTitleBar": "False",
  "FIntFullscreenTitleBarTriggerDelayMillis": "3600000",
  "FFlagDisablePostFx": "True",
  "DFFlagDisableDPIScale": "True",
  "DFIntMaxMissedWorldStepsRemembered": "1000",
  "DFIntNumAssetsMaxToPreload": "9999999",
  "DFIntAssetPreloading": "9999999"
}
```
### Improve Animation Speed, Visual Fidelity, and Ping
``` json
{
    "FFlagSimEnableDCD10": "True",
    "FFlagDebugGraphicsPreferD3D11FL10": "True",
    "DFIntBufferCompressionLevel": "0",
    "DFIntBufferCompressionThreshold": "100",
    "DFIntPerformanceControlFrameTimeMax": "1",
    "DFIntPerformanceControlFrameTimeMaxUtility": "-1",
    "FFlagPushFrameTimeToHarmony": "True",
    "FFlagUISUseLastFrameTimeInUpdateInputSignal": "True",
    "DFIntAnimatorThrottleMaxFramesToSkip": "1",
    "DFIntNumFramesAllowedToBeAboveError": "1",
    "DFIntVisibilityCheckRayCastLimitPerFrame": "10",
    "DFIntNetworkSchemaCompressionRatio": "100",
    "DFIntTimeBetweenSendConnectionAttemptsMS": "200"
}
```
### Extreme Latency
``` json
{
    "DFIntLargePacketQueueSizeCutoffMB": "1000",
    "DFIntMaxProcessPacketsJobScaling": "10000",
    "DFIntMaxProcessPacketsStepsAccumulated": "0",
    "DFIntMaxProcessPacketsStepsPerCyclic": "5000",
    "DFIntMegaReplicatorNetworkQualityProcessorUnit": "10"
}
```
### Network CPU RSS Tweaks
``` json
{
    "DFIntPhysicsReceiveNumParallelTasks": "20",
    "DFIntPhysicsAnalyticsHighFrequencyIntervalSec": "20",
    "FFlagSimAdaptiveMinorOptimizations": "True",
    "FIntSimWorldTaskQueueParallelTasks": "20",
    "FIntSmoothClusterTaskQueueMaxParallelTasks": "20",
    "DFIntReplicationDataCacheNumParallelTasks": "20",
    "DFIntMegaReplicatorNumParallelTasks": "20"
}
```
### V1
###### very low quality for performance, by espresso-soft
``` json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
    "DFIntTaskSchedulerTargetFps": "9999",
    "FFlagDebugRenderingSetDeterministic": "True",
    "DFFlagDebugRenderForceTechnologyVoxel": "True",
    "FIntRenderShadowIntensity": "0",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "DFFlagDisableDPIScale": "True",
    "DFIntDebugFRMQualityLevelOverride": "1",
    "FFlagCommitToGraphicsQualityFix": "True",
    "FFlagFixGraphicsQuality": "True",
    "FFlagGlobalWindRendering": "False",
    "FIntRenderLocalLightUpdatesMax": "8",
    "FIntRenderLocalLightUpdatesMin": "6",
    "FIntRenderLocalLightFadeInMs": "-1",
    "FFlagDisablePostFx": "True",
    "DFFlagDebugPauseVoxelizer": "True",
    "FFlagDebugSkyGray": "True",
    "FFlagFastGPULightCulling3": "True",
    "DFIntMaxFrameBufferSize": "4",
    "FIntTerrainArraySliceSize": "4",
    "DFIntTextureCompositorActiveJobs": "0",
    "FIntDebugTextureManagerSkipMips": "8",
    "FIntFRMMinGrassDistance": "0",
    "FIntFRMMaxGrassDistance": "0",
    "FIntRenderGrassDetailStrands": "0",
    "FIntRenderGrassHeightScaler": "0",
    "FIntRenderShadowmapBias": "-1",
    "FFlagAdServiceEnabled": "False",
    "DFIntAnimationLodFacsDistanceMin": "0",
    "DFIntAnimationLodFacsDistanceMax": "0",
    "DFIntAnimationLodFacsVisibilityDenominator": "0",
    "FFlagEnableInGameMenuChromeABTest2": "False",
    "FFlagEnableReportAbuseMenuRoactABTest2": "False",
    "FFlagEnableInGameMenuChromeABTest3": "False",
    "FFlagUserShowGuiHideToggles": "True",
    "GuiHidingApiSupport2": "True",
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000"
}
```
### V2
###### by espresso-soft
``` json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
    "DFIntTaskSchedulerTargetFps": "9999",
    "FFlagRenderFixFog": "True",
    "FFlagDebugCheckRenderThreading": "True",
    "FFlagRenderDebugCheckThreading2": "True",
    "FIntRenderShadowIntensity": "0",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "DFFlagDisableDPIScale": "True",
    "FFlagCommitToGraphicsQualityFix": "True",
    "FFlagFixGraphicsQuality": "True",
    "FIntRenderLocalLightUpdatesMax": "6",
    "FIntRenderLocalLightUpdatesMin": "4",
    "FIntRenderLocalLightFadeInMs": "0",
    "FFlagDisablePostFx": "True",
    "FFlagNewLightAttenuation": "True",
    "FFlagDebugForceFSMCPULightCulling": "True",
    "DFIntMaxFrameBufferSize": "6",
    "DFFlagTextureQualityOverrideEnabled": "True",
    "DFIntTextureQualityOverride": "3",
    "FIntFRMMinGrassDistance": "0",
    "FIntFRMMaxGrassDistance": "0",
    "FIntRenderGrassDetailStrands": "0",
    "FIntDebugForceMSAASamples": "0",
    "FFlagGameBasicSettingsFramerateCap5": "False",
    "FFlagUserShowGuiHideToggles": "True",
    "FFlagGuiHidingApiSupport2": "True",
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000",
    "DFIntTimestepArbiterThresholdCFLThou": "300",
    "FFlagAdServiceEnabled": "False",
    "FFlagDebugDisableTelemetryEphemeralCounter": "True",
    "FFlagDebugDisableTelemetryEphemeralStat": "True",
    "FFlagDebugDisableTelemetryEventIngest": "True",
    "FFlagDebugDisableTelemetryPoint": "True",
    "FFlagDebugDisableTelemetryV2Counter": "True",
    "FFlagDebugDisableTelemetryV2Event": "True",
    "FFlagDebugDisableTelemetryV2Stat": "True",
    "DFIntDefaultTimeoutTimeMs": "10000",
    "FFlagEnableQuickGameLaunch": "True",
    "DFIntAnimationLodFacsDistanceMin": "0",
    "DFIntAnimationLodFacsDistanceMax": "0",
    "DFIntAnimationLodFacsVisibilityDenominator": "0",
    "FFlagHandleAltEnterFullscreenManually": "False",
    "FIntRobloxGuiBlurIntensity": "0",
    "FFlagErrorPromptResizesHeight": "False",
    "FFlagNewCameraControls": "True",
    "DFIntS2PhysicsSenderRate": "10000"
}
```
### v2 modified
###### espresso-soft's v2, not youtuber optimizations.
##### use lower ping for lower ping.
##### early fflag optimization, do not use if your using a game with heavy light.
``` json
{
  "FLogNetwork": "7",
  "DFIntAnimationLodFacsVisibilityDenominator": "0",
  "FFlagDebugDisableTelemetryEventIngest": "True",
  "DFFlagDebugRenderForceTechnologyVoxel": "True",
  "DFIntPhysicsAnalyticsHighFrequencyIntervalSec": "20",
  "FFlagGuiHidingApiSupport2": "True",
  "FFlagEnableInGameMenuChrome": "False",
  "FFlagEnableV3MenuABTest3": "False",
  "FIntTerrainArraySliceSize": "4",
  "DFIntTextureQualityOverride": "3",
  "DFIntAnimationLodFacsDistanceMin": "0",
  "FIntRenderShadowIntensity": "0",
  "FFlagDebugDisableTelemetryV2Event": "True",
  "FFlagErrorPromptResizesHeight": "False",
  "FFlagEnableInGameMenuControls": "True",
  "FFlagDebugCheckRenderThreading": "True",
  "FIntRenderLocalLightUpdatesMax": "6",
  "DFIntMaxMissedWorldStepsRemembered": "1000",
  "FIntSmoothClusterTaskQueueMaxParallelTasks": "20",
  "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
  "FFlagDisablePostFx": "True",
  "DFFlagTextureQualityOverrideEnabled": "True",
  "FIntFullscreenTitleBarTriggerDelayMillis": "3600000",
  "DFFlagDisableDPIScale": "True",
  "DFIntPhysicsReceiveNumParallelTasks": "20",
  "FFlagDebugDisableTelemetryEphemeralStat": "True",
  "FIntRobloxGuiBlurIntensity": "0",
  "FFlagUserRaycastPerformanceImprovements": "true",
  "FIntDebugForceMSAASamples": "0",
  "FFlagUserShowGuiHideToggles": "True",
  "FFlagEnableInGameMenuChromeABTest4": "False",
  "FFlagDebugDisableTelemetryV2Counter": "True",
  "DFIntCanHideGuiGroupId": "32380007",
  "FFlagEnableMenuControlsABTest": "False",
  "DFIntDebugFRMQualityLevelOverride": "1",
  "FIntFRMMinGrassDistance": "0",
  "FIntSimWorldTaskQueueParallelTasks": "20",
  "FFlagDebugForceFSMCPULightCulling": "True",
  "DFIntTaskSchedulerTargetFps": "0",
  "FFlagEnableInGameMenuChromeABTest3": "False",
  "DFIntAnimationLodFacsDistanceMax": "0",
  "FFlagDebugDisableTelemetryEphemeralCounter": "True",
  "FFlagEnableInGameMenuModernization": "True",
  "FFlagSimAdaptiveMinorOptimizations": "True",
  "DFIntConnectionMTUSize": "900",
  "FIntRenderGrassDetailStrands": "0",
  "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
  "FIntNewInGameMenuPercentRollout3": "0",
  "FFlagHandleAltEnterFullscreenManually": "False",
  "DFIntDefaultTimeoutTimeMs": "10000",
  "FFlagDebugDisableTelemetryV2Stat": "True",
  "FFlagGameBasicSettingsFramerateCap5": "True",
  "DFIntReplicationDataCacheNumParallelTasks": "20",
  "FFlagRenderFixFog": "True",
  "FFlagNewLightAttenuation": "True",
  "DFIntMegaReplicatorNumParallelTasks": "20",
  "FIntRenderLocalLightUpdatesMin": "4",
  "DFIntAssetPreloading": "9999999",
  "DFIntMaxFrameBufferSize": "6",
  "FFlagRenderDebugCheckThreading2": "True",
  "FIntRenderLocalLightFadeInMs": "0",
  "FFlagCommitToGraphicsQualityFix": "True",
  "FFlagEnableQuickGameLaunch": "True",
  "DFIntTimestepArbiterThresholdCFLThou": "300",
  "DFIntS2PhysicsSenderRate": "10000",
  "FFlagDebugGraphicsDisableDirect3D11": "True",
  "FFlagNewCameraControls": "True",
  "FFlagFixGraphicsQuality": "True",
  "FFlagAdServiceEnabled": "False",
  "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
  "FIntFRMMaxGrassDistance": "0",
  "FFlagFRMRefactor": "false",
  "DFIntNumAssetsMaxToPreload": "9999999",
  "FFlagDebugDisableTelemetryPoint": "True",
  "DFFlagDebugPauseVoxelizer": "True",
  "FFlagDebugGraphicsPreferVulkan": "True",
  "FFlagDebugForceFutureIsBrightPhase2": "True",
  "FFlagUserUpdateInputConnections": "true",
  "DFIntHttpRbxApiMaxBudgetMultiplier": "2",
  "DFIntHttpRbxApiJobFrequencyInSeconds": "60",
  "DFIntHttpRbxApiClientPerMinuteRequestLimit": "60",
  "DFIntHttpRbxApiMaxRetryBudgetPerMinute": "60",
  "DFIntHttpRbxApiMaxRetryCount": "3",
  "DFIntHttpRbxApiMaxRetryQueueSize": "1000",
  "DFIntHttpRbxApiMaxSyncRetries": "3",
  "DFIntHttpRbxApiPerMinuteRequestLimit": "60",
  "DFIntHttpRbxApiSameUrlRequestLimit": "30",
  "DFIntHttpRbxApiServiceDecaySeconds": "300",
  "DFIntHttpRbxApiMaxThrottledQueue": "500",
  "DFFlagSimOptimizeSetSize": "True",
  "FIntDirectionalAttenuationMaxPoints": "50",
  "FFlagRenderCBRefactor2": "True",
  "FFlagLuaAppLegacyInputSettingRefactor": "True",
  "FFlagRenderShadowSkipHugeCulling": "true",
  "FFlagShoeSkipRenderMesh": "false",
  "FFlagEnableNewChatTabExperiment5": "False",
  "FIntRakNetResendBufferArrayLength": "128",
  "FFlagOptimizeNetwork": "True",
  "FFlagOptimizeNetworkRouting": "True",
  "FFlagOptimizeNetworkTransport": "True",
  "FFlagOptimizeServerTickRate": "True",
  "DFIntServerPhysicsUpdateRate": "60",
  "DFIntServerTickRate": "60",
  "DFIntRakNetResendRttMultiple": "1",
  "DFIntRaknetBandwidthPingSendEveryXSeconds": "1",
  "DFIntOptimizePingThreshold": "50",
  "DFIntPlayerNetworkUpdateQueueSize": "20",
  "DFIntPlayerNetworkUpdateRate": "60",
  "DFIntNetworkPrediction": "120",
  "DFIntNetworkLatencyTolerance": "1",
  "DFIntMinimalNetworkPrediction": "0.1",
  "FFlagMovePrerender": "True"
}
```
### youtuber optimizations
### v1
###### [video](https://www.youtube.com/watch?v=fj0zVi6UG9A)
##### Basic FPS Boosting Flaglist
``` json
{
  "FFlagHandleAltEnterFullscreenManually": "False",
  "FLogNetwork": "7",
  "FIntDebugForceMSAASamples": "0",
  "FIntRenderShadowIntensity": "0",
  "FFlagDisablePostFx": "True",
  "FIntTerrainArraySliceSize": "0",
  "DFIntTaskSchedulerTargetFps": "160",
  "FFlagDebugGraphicsPreferD3D11": "True",
  "FIntFullscreenTitleBarTriggerDelayMillis": "3600000",
  "FFlagNewLightAttenuation": "True",
  "DFIntDebugFRMQualityLevelOverride": "1",
  "FFlagDebugDisplayFPS": "True",
  "FFlagGlobalWindRendering": "False",
  "FFlagGlobalWindActivated": "False",
  "FIntFRMMinGrassDistance": "0",
  "FIntFRMMaxGrassDistance": "0",
  "FIntRenderGrassDetailStrands": "0",
  "FIntRenderGrassHeightScaler": "0"
}
```
### v2
##### Will literally disable major load components like textures, lighting, skybox, UI, etc.
``` json
{
  "FFlagHandleAltEnterFullscreenManually": "False",
  "FLogNetwork": "7",
  "FIntDebugForceMSAASamples": "0",
  "FIntRenderShadowIntensity": "0",
  "FFlagDisablePostFx": "True",
  "FIntTerrainArraySliceSize": "4",
  "DFIntTaskSchedulerTargetFps": "160",
  "FFlagDebugGraphicsPreferD3D11": "True",
  "FIntFullscreenTitleBarTriggerDelayMillis": "3600000",
  "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
  "FFlagNewLightAttenuation": "True",
  "DFIntDebugFRMQualityLevelOverride": "1",
  "FFlagDebugDisplayFPS": "True",
  "FFlagGlobalWindRendering": "False",
  "FFlagGlobalWindActivated": "False",
  "FIntFRMMinGrassDistance": "0",
  "FIntFRMMaxGrassDistance": "0",
  "FIntRenderGrassDetailStrands": "0",
  "FIntRenderGrassHeightScaler": "0",
  "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
  "DFFlagDebugPauseVoxelizer": "True",
  "FFlagDebugSkyGray": "True",
  "DFIntCSGLevelOfDetailSwitchingDistance": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0",
  "FFlagDebugForceFSMCPULightCulling": "True",
  "DFIntPerformanceControlTextureQualityBestUtility": "-1",
  "DFIntTextureCompositorActiveJobs": "0",
  "DFFlagTextureQualityOverrideEnabled": "True",
  "DFIntTextureQualityOverride": "0",
  "FFlagUpdateHealthBar": "False"
}
```
### v1 modified
###### making in a week or so, make an issue if you have one.
### v2 modified
###### making in a week or so, make an issue if you have one.
### RCOOL OPTIMIZATIONS (MAY BE OLD)
``` json
{
    "FFlagHandleAltEnterFullscreenManually": "False",
    "FLogNetwork": "7",
    "DFIntTaskSchedulerTargetFps": "9999",
    "FFlagFixGraphicsQuality": "True",
    "FFlagDebugDisableTelemetryEphemeralCounter": "True",
    "FFlagDebugDisableTelemetryEphemeralStat": "True",
    "FIntRenderLocalLightFadeInMs": "0",
    "FFlagDebugDisableTelemetryEventIngest": "True",
    "FFlagDebugDisableTelemetryPoint": "True",
    "FFlagDebugDisableTelemetryV2Counter": "True",
    "FFlagDebugDisableTelemetryV2Event": "True",
    "FFlagDebugDisableTelemetryV2Stat": "True",
    "FStringPartTexturePackTable2022": "{\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873284556\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[254,254,254,7]}}",
    "FStringPartTexturePackTablePre2022": "{\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://7547304948\u0022,\u0022rbxassetid://7546645118\u0022],\u0022color\u0022:[254,254,254,7]}}",
    "FStringTerrainMaterialTable2022": "",
    "FStringTerrainMaterialTablePre2022": "",
    "FFlagGlobalWindActivated": "False",
    "FFlagEnableBetaFacialAnimation2": "False",
    "FFlagFacialAnimationSupport1": "False",
    "DFIntAnimationLodFacsDistanceMin": "0",
    "DFIntAnimationLodFacsDistanceMax": "0",
    "DFIntAnimationLodFacsVisibilityDenominator": "0",
    "DFFlagEnableDynamicHeadByDefault": "False",
    "FIntRobloxGuiBlurIntensity": "0",
    "FFlagDebugRenderingSetDeterministic": "True",
    "DFIntCSGLevelOfDetailSwitchingDistance": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0",
    "FIntRenderLocalLightUpdatesMax": "1",
    "FIntRenderLocalLightUpdatesMin": "1",
    "FFlagAdServiceEnabled": "False",
    "FFlagFastGPULightCulling3": "True",
    "FFlagNewLightAttenuation": "True",
    "FFlagGlobalWindRendering": "False",
    "FIntRenderShadowIntensity": "0",
    "FIntRenderShadowmapBias": "1",
    "FIntDebugForceMSAASamples": "-1",
    "FIntFRMMinGrassDistance": "0",
    "FFlagLuaAppUseUIBloxColorPalettes1": "True",
    "FFlagEnableCommandAutocomplete": "True",
    "FFlagUIBloxUseNewThemeColorPalettes": "True",
    "FIntFRMMaxGrassDistance": "0",
    "FFlagSoundsUsePhysicalVelocity": "True",
    "FIntRenderGrassDetailStrands": "0",
    "FFlagChromeBetaFeature": "False",
    "FFlagEnableInGameMenuChromeABTest2": "False",
    "FFlagEnableReportAbuseMenuRoactABTest2": "False",
    "FFlagEnableChromePinnedChat": "False",
    "FFlagEnableInGameMenuChrome": "False",
    "FFlagEnableInGameMenuChromeABTest": "False",
    "FFlagEnableInGameMenuChromeSignalAPI": "False",
    "FFlagPlayerListChromePushdown": "False",
    "FStringEnableChromePinnedChatForcedUserIds": "1",
    "FStringGameMenuChromeForcedUserIds": "1",
    "FFlagVoiceBetaBadge": "False",
    "FFlagTopBarUseNewBadge": "False",
    "FFlagEnableBetaBadgeLearnMore": "False",
    "FFlagBetaBadgeLearnMoreLinkFormview": "False",
    "FFlagControlBetaBadgeWithGuac": "False",
    "FStringVoiceBetaBadgeLearnMoreLink": "null",
    "FIntRenderGrassHeightScaler": "0",
    "DFFlagDebugRenderForceTechnologyVoxel": "True",
    "DFFlagDisableDPIScale": "True",
    "DFIntTextureCompositorActiveJobs": "0",
    "FFlagCoreGuiTypeSelfViewPresent": "False",
    "DFIntDebugFRMQualityLevelOverride": "1",
    "FFlagDisableNewIGMinDUA": "True",
    "FFlagPreloadAllFonts": "True",
    "FFlagCommitToGraphicsQualityFix": "True",
    "FFlagDebugSkyGray": "True",
    "DFIntMaxFrameBufferSize": "4",
    "FFlagRenderGpuTextureCompressor": "True",
    "FFlagGpuGeometryManager7": "True",
    "DFFlagPredictedOOM": "False",
    "DFIntPredictedOOMPercent": "0",
    "FFlagDisablePostFx": "True",
    "FFlagEnableQuickGameLaunch": "True",
    "DFFlagDebugPauseVoxelizer": "True",
    "FIntTerrainArraySliceSize": "4",
    "DFFlagTextureQualityOverrideEnabled": "True",
    "DFIntTextureQualityOverride": "1",
    "FFlagEnableAudioOutputDevice": "False"
}
```

### you finished??
### heres the code frequency:
 ![image](https://github.com/user-attachments/assets/7110f208-5ba5-445f-9ce8-6e66fa9850ca)


 ### no telemetry
 ``` json
{
"DFStringTelegrafHTTPTransportUrl": "n.google.com",
"DFStringTelemetryV2Url": "n.google.com",
"DFStringTelegrafAddress": "0.0.0.0",
"DFStringRobloxAnalyticsURL": "n.google.com",
"FFlagEnableBooleanRobloxTelemetry": false,
"FFlagLuaAppChallengeMoreTelemetryEnabled": false,
"FFlagLuaAppLogoutTelemetry": false,
"FFlagReportRenderDistanceTelemetry": false,
"FFlagSocialAnalyticsSupportTelemetry": false,
"FFlagSTUDIOPLAT34382ANRMoreTelemetry": false,
"FFlagTimeAndNewJoinDataTelemetry": false,
"FFlagVideoCaptureFailureTelemetry": false,
"FFlagVoiceChatDontSendTelemetryForPubIceTrickle": true,
"FFlagVoiceChatEnableRobloxTelemetryServiceInitEvent": false,
"FIntBootstrapperTelemetryReportingHundredthsPercentage": 0,
"FIntConnectionTelemetryPollIntervalMS": 32700000,
"FIntHttpWrapperTelemetryHundredthsPercent": 0,
"FIntUserActionTrackerTelemetryHundredthsPercent": 0,
"DFFlagAddDynamicHeadTelemetryToSessionTracking2": false,
"DFFlagAddPlaySessionIdTelemetry": false,
"DFFlagAudioDeviceTelemetry": false,
"DFFlagBrowserTrackerIdTelemetryEnabled": false,
"DFFlagClientLightingTechnologyChangedTelemetryTrackTimeSpent": false,
"DFFlagClientRolloutPhaseTelemetry": false,
"DFFlagEnableTelemetryV2FRMStats": false,
"DFFlagFFlagRolloutDuplicateRobloxTelemetryCountersEnabled": false,
"DFFlagFFlagRolloutDuplicateTelemetryCountersEnabled": false,
"DFFlagGraphicsQualityUsageTelemetry": false,
"DFFlagReportLegacyFRMStatsToTelemetryV2": false,
"DFFlagSessionTelemetryLayeredClothing": false,
"DFFlagVoiceReliabilityTelemetryEventIngest": false,
"FFlagDebugDisableTelemetryEphemeralCounter": "True",
"FFlagDebugDisableTelemetryEphemeralStat": "True",
"FFlagDebugDisableTelemetryEventIngest": "True",
"FFlagDebugDisableTelemetryPoint": "True",
"FFlagDebugDisableTelemetryV2Counter": "True",
"FFlagDebugDisableTelemetryV2Event": "True",
"FFlagDebugDisableTelemetryV2Stat": "True"
}
```
### It improves gameplay, giving strong FPS and good ping.
# prepare
```json
{
  "FLogNetwork": "7",
  "FFlagHandleAltEnterFullscreenManually": "False",
  "FFlagHighlightOutlinesOnMobile": "True",
  "DFIntHttpRbxApiPerMinuteRequestLimit": "60",
  "FIntRakNetResendBufferArrayLength": "128",
  "FFlagSimIslandizerManager": "false",
  "DFStringHttpPointsReporterUrl": "null",
  "DFIntHttpRbxApiMaxRetryCount": "3",
  "FFlagTweenOptimizations": "True",
  "DFIntTaskSchedulerTargetFps": "9999999",
  "FFlagFastGPULightCulling3": "True",
  "DFStringAltTelegrafHTTPTransportUrl": "null",
  "FFlagUseNewAnimationSystem": "False",
  "DFIntHttpRbxApiMaxRetryBudgetPerMinute": "60",
  "DFIntHttpRbxApiMaxRetryQueueSize": "1000",
  "FFlagAdServiceEnabled": "False",
  "FFlagFixMeshPartScaling": "False",
  "DFIntServerTickRate": "60",
  "FFlagDebugDisplayFPS": "False",
  "FIntTerrainArraySliceSize": "0",
  "FFlagDebugDisableTelemetryV2Counter": "True",
  "DFFlagEnableLightstepReporting2": "False",
  "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
  "FStringGamesUrlPath": "/games/",
  "FFlagDisablePostFx": "True",
  "FFlagOptimizeServerTickRate": "True",
  "DFIntServerPhysicsUpdateRate": "60",
  "DFStringLightstepHTTPTransportUrlPath": "null",
  "FFlagDebugDisableTelemetryPoint": "True",
  "DFIntHttpRbxApiSameUrlRequestLimit": "30",
  "FFlagPreloadAllFonts": "True",
  "FFlagDebugDisableTelemetryEphemeralStat": "True",
  "FStringCoreScriptBacktraceErrorUploadToken": "null",
  "DFIntRakNetResendRttMultiple": "1",
  "DFIntHttpRbxApiMaxThrottledQueue": "500",
  "FFlagDebugDisableTelemetryV2Event": "True",
  "DFIntConnectionMTUSize": "690",
  "DFFlagDebugPerfMode": "True",
  "FFlagOptimizeNetworkTransport": "True",
  "DFIntPlayerNetworkUpdateQueueSize": "20",
  "DFFlagDisableDPIScale": "False",
  "DFFlagBrowserTrackerIdTelemetryEnabled": "False",
  "DFIntHttpRbxApiJobFrequencyInSeconds": "60",
  "FFlagAnimatePhysics": "False",
  "DFStringLightstepHTTPTransportUrlHost": "null",
  "DFIntHttpRbxApiMaxBudgetMultiplier": "2",
  "FFlagOptimizeEmotes": "False",
  "FFlagOptimizeNetworkRouting": "True",
  "DFIntRenderingThrottleDelayInMS": "1",
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0",
  "FIntFontSizePadding": "4",
  "DFStringLightstepToken": "null",
  "FFlagUseDynamicSun": "False",
  "DFStringCrashUploadToBacktraceWindowsPlayerToken": "null",
  "FFlagOptimizeNetwork": "True",
  "DFIntOptimizePingThreshold": "50",
  "FFlagUseUnifiedRenderStepped": "False",
  "FFlagCommitToGraphicsQualityFix": "True",
  "DFIntNetworkLatencyTolerance": "1",
  "DFIntHttpRbxApiClientPerMinuteRequestLimit": "60",
  "FFlagEnableNewHeapSnapshots": "False",
  "FFlagEnableTerrainOptimizations": "True",
  "DFFlagBaseNetworkMetrics": "False",
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
  "DFIntS2PhysicsSenderRate": "38760",
  "DFIntHttpRbxApiMaxSyncRetries": "3",
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
  "FFlagNewLightAttenuation": "True",
  "FFlagUseDeferredContext": "False",
  "DFIntClientLightingTechnologyChangedTelemetryHundredthsPercent": "0",
  "FFlagFixScalingModelRendering": "False",
  "DFIntRaknetBandwidthPingSendEveryXSeconds": "1",
  "FFlagDebugDisableTelemetryEphemeralCounter": "True",
  "DFIntHttpRbxApiServiceDecaySeconds": "300",
  "DFIntLightstepHTTPTransportHundredthsPercent2": "0",
  "FFlagEnableHumanoidLuaSideCaching": "False",
  "DFIntRunningBaseOrientationP": "450",
  "FFlagNewNetworking": "False",
  "FFlagEnableNewInput": "True",
  "FFlagDebugCrashReports": "False",
  "DFFlagDisableFastLogTelemetry": "True",
  "DFStringRobloxAnalyticsURL": "null",
  "FFlagLuaAppSystemBar": "False",
  "FFlagDebugDisableTelemetryEventIngest": "True",
  "DFIntNewRunningBaseAltitudeD": "50",
  "DFFlagDebugPauseVoxelizer": "True",
  "DFStringCrashUploadToBacktraceMacPlayerToken": "null",
  "FFlagFixGraphicsQuality": "True",
  "FFlagUseParticlesV2": "False",
  "DFIntCSGLevelOfDetailSwitchingDistance": "1",
  "DFStringAltHttpPointsReporterUrl": "null",
  "DFIntNetworkPrediction": "120",
  "FIntRenderShadowIntensity": "0",
  "DFStringTelemetryV2Url": "null",
  "DFStringCrashUploadToBacktraceBaseUrl": "null",
  "FFlagDebugSkyGray": "True",
  "DFStringTelegrafHTTPTransportUrl": "null",
  "DFIntPlayerNetworkUpdateRate": "60",
  "FFlagDebugDisableTelemetryV2Stat": "True",
  "FFlagEnableTerrainFoliageOptimizations": "True",
  "FFlagEnableLightAttachToPart": "False",
  "DFIntCanHideGuiGroupId": "32380007",
  "DFIntMinimalNetworkPrediction": "1",
  "FFlagGameBasicSettingsFramerateCap5": "False",
  "FStringDebugGraphicsPreferredGPUName": "AMD Radeon RX 7600",
  "FFlagEnableInGameMenuChromeABTest2": "False",
  "FStringPartTexturePackTable2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://98732842556\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[255, 255, 255, 255]}}",
  "FFlagEnableV3MenuABTest3": "False",
  "FFlagEnableMenuModernizationABTest2": "False",
  "FFlagEnableMenuModernizationABTest": "False",
  "FFlagEnableMenuControlsABTest": "False",
  "FFlagEnableInGameMenuControls": "True",
  "FFlagDisableNewIGMinDUA": "True",
  "FFlagEnableInGameMenuModernization": "True",
  "FIntFRMMinGrassDistance": "0",
  "FIntFRMMaxGrassDistance": "0",
  "FIntRenderGrassDetailStrands": "0",
  "FintRenderGrassHeightScaler": "0",
  "DFIntDebugFRMQualityLevelOverride": "1",
  "FFlagDebugGraphicsPreferD3D11FL10": "True",
  "FIntDebugForceMSAASamples": "0",
  "DFLogHttpTraceLight": "0",
  "FFlagEnableAccessibilitySettingsAPIV2": "True",
  "FFlagEnableAccessibilitySettingsEffectsInCoreScripts2": "True",
  "FFlagCoreGuiTypeSelfViewPresent": "False",
  "DFIntTextureQualityOverride": "6",
  "FFlagInGameMenuV1FullScreenTitleBar": "False",
  "DFFlagTextureQualityOverrideEnabled": "True",
  "GoogleAnalyticsAccountPropertyIDPlayer": "null",
  "FIntCameraMaxZoomDistance": "99999",
  "FFlagVoiceBetaBadge": "false",
  "FFlagEnableInGameMenuV3": "False",
  "FFlagCloudsReflectOnWater": "True",
  "FFlagEnableAccessibilitySettingsInExperienceMenu2": "True",
  "FFlagEnableAccessibilitySettingsEffectsInExperienceChat": "True",
  "GoogleAnalyticsAccountPropertyID": "null",
  "FFlagDontCreatePingJob": "True",
  "\u0022FIntCameraMaxZoomDistance\u0022: \u002299999\u0022": "99999",
  "DFStringAnalyticsEventStreamUrlEndpoint": "opt-out",
  "FFlagEnableBatteryStateLogger": "False",
  "FStringTerrainMaterialTablePre2022": "",
  "FIntMeshContentProviderForceCacheSize": "268435456",
  "DFIntCrashReportingHundredthsPercentage": "0",
  "FStringPerformanceSendMeasurementAPISubdomain": "opt-out",
  "FIntStartupInfluxHundredthsPercentage": "0",
  "FFlagRenderGpuTextureCompressor": "True",
  "FFlagImmersiveAdsWhitelistDisabled": "False",
  "DFFlagAddUserIdToSessionTracking": "False",
  "\u0022DFIntCSGLevelOfDetailSwitchingDistanceL23\u0022": "0",
  "FIntTerrainOTAMaxTextureSize": "1024",
  "FIntReportDeviceInfoRollout": "0",
  "DFFlagESGamePerfMonitorEnabled": "False",
  "FStringTerrainMaterialTable2022": "",
  "DFIntPredictedOOMPercent": "0",
  "FIntDefaultMeshCacheSizeMB": "256",
  "FStringImmersiveAdsUniverseWhitelist": "0",
  "FIntBootstrapperTelemetryReportingHundredthsPercentage": "0",
  "FIntAbuseReportScreenshotMaxSize": "0",
  "FIntLinkBrowserTrackerToDeviceRollout": "0",
  "FFlagEnableAudioOutputDevice": "false",
  "FFlagDebugDisableOTAMaterialTexture": "true",
  "FStringErrorUploadToBacktraceBaseUrl": "https://opt-out.roblox.com",
  "FFlagGraphicsCheckComputeSupport": "True",
  "DFFlagGpuVsCpuBoundTelemetry": "False",
  "FFlagLocServicePerformanceAnalyticsEnabled": "False",
  "FFlagEnableQuickGameLaunch": "True",
  "FFlagTrackMacWebLaunchFlow": "False",
  "FFlagPreloadMinimalFonts": "True",
  "DFFlagPredictedOOM": "False",
  "\u0022DFIntCSGLevelOfDetailSwitchingDistanceL12\u0022": "0",
  "DFIntWriteFullDmpPercent": "0",
  "FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0",
  "DFFlagHttpCacheCleanBasedOnMemory": "True",
  "DFIntDetectCrashEarlyPercentage": "0",
  "DFFlagEnableFmodErrorsTelemetry": "False",
  "FIntHSRClusterSymmetryDistancePercent": "10000",
  "FFlagAvatarChatSettingsEnabled2": "False",
  "FFlagReportFpsAndGfxQualityPercentiles": "False",
  "DFFlagDebugAnalyticsSendUserId": "False",
  "FFlagFacialAnimationStreamingServiceUniverseSettingsEnableAudio": "False",
  "FFlagRenderPerformanceTelemetry": "False",
  "DFLogHttpTrace": "0",
  "FFlagTrackPlaceIdForCrashEnabled": "False",
  "DFFlagAvatarChatServiceUserPermissionsAudioEligible": "False",
  "FFlagVoiceChatServiceManagerUseAvatarChat": "False",
  "FFlagAddGameInstanceIdToSessionTracking": "False",
  "FFlagDebugForceChatDisabled": "False",
  "DFFlagAddPublicGettersForGfxQualityAndFpsForTelemCounters2": "False",
  "FFlagGraphicsEnableD3D10Compute": "True",
  "DFFlagAudioDeviceTelemetry": "False",
  "DFLogBatchAssetApiLog": "3",
  "DFFlagAvatarChatServiceUserPermissionsAudioOptIn": "False",
  "FFlagDebugGraphicsDisableDirect3D11": "False",
  "DFIntHttpCurlConnectionCacheSize": "134217728",
  "DFFlagEnableMemProfilingStorePlaceId": "False",
  "FFlagGraphicsSettingsOnlyShowValidModes": "True",
  "DFLogHttpTraceError": "0",
  "DFFlagQueueDataPingFromSendData": "True",
  "FFlagEnableAdsAPI": "False",
  "DFFlagCrashUploadFullDumps": "False",
  "FFlagAnimationClipMemCacheEnabled": "True",
  "FFlagDebugRenderingSetDeterministic": "True",
  "DFStringRobloxAnalyticsSubDomain": "opt-out",
  "DFIntUserIdPlayerNameCacheSize": "33554432",
  "FFlagFacialAnimationStreamingServiceUserSettingsOptInAudio": "False",
  "FFlagAudioDeviceTelemetry": "false",
  "FFlagWindowsLaunchAnalytics": "False",
  "FFlagDebugGraphics": "False",
  "FIntUITextureMaxRenderTextureSize": "1024",
  "FFlagFacialAnimationStreamingServiceUniverseSettingsEnableVideo": "False",
  "FFlagGlobalWindRendering": "false",
  "FFlagGraphicsGLEnableHQShadersExclusion": "False",
  "DFFlagEnableGCapsHardwareTelemetry": "False",
  "DFIntUserIdPlayerNameLifetimeSeconds": "86400",
  "DFIntCrashUploadToBacktracePercentage": "0",
  "FFlagBatchAssetApi": "True",
  "DFFlagEnableMemProfilingOutsideClient": "False",
  "FStringPartTexturePackTablePre2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873266399\u0022,\u0022rbxassetid://9438410239\u0022],\u0022color\u0022:[238,238,238,255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9930003180\u0022,\u0022rbxassetid://9438410548\u0022],\u0022color\u0022:[227,227,228,234]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920482224\u0022,\u0022rbxassetid://9438413638\u0022],\u0022color\u0022:[160,160,158,238]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920482992\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[229,214,205,227]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9919719550\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[218,219,219,243]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920484334\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[225,225,224,255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920485426\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[76,79,81,156]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://10237721036\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[210,210,210,255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920517963\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[221,221,221,255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920518995\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[225,229,229,243]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873284556\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[254,254,254,7]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920550720\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[210,206,200,255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920552044\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[196,196,189,241]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920554695\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[165,165,160,240]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920556429\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[235,239,241,248]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920558145\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[182,178,175,234]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920561624\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[250,248,243,250]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873292869\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[181,183,193,249]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920574966\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[226,226,226,255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920578676\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[193,192,193,252]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920580094\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[218,218,219,236]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920581197\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[204,203,201,234]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://9475422736\u0022],\u0022color\u0022:[255,255,255,255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://10129366149\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[211,211,210,248]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920589512\u0022,\u0022rbxassetid://9439557520\u0022],\u0022color\u0022:[206,177,163,180]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920590478\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[249,249,249,255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920591862\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[218,216,210,240]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920596353\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[241,234,230,246]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920600052\u0022,\u0022rbxassetid://9439613006\u0022],\u0022color\u0022:[235,234,235,254]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920620451\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[239,240,240,255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920625499\u0022,\u0022rbxassetid://9439649548\u0022],\u0022color\u0022:[217,209,208,255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9920626896\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[207,208,206,254]}}",
  "\u0022DFIntCSGLevelOfDetailSwitchingDistanceL34\u0022": "0",
  "FIntTaskSchedulerAutoThreadLimit": "8",
  "FFlagDebugGraphicsDisableOpenGL": "True",
  "FFlagTrackWinWebLaunchFlow": "False",
  "FFlagDebugGraphicsCrashOnLeaks": "False",
  "FIntLmsClientRollout2": "0",
  "FIntFlagUpdateVersion": "132",
  "FIntRenderShadowmapBias": "0",
  "\u0022DFIntCSGLevelOfDetailSwitchingDistance\u0022": "0",
  "DFFlagEnableHardwareTelemetry": "false",
  "FIntRenderEnableGlobalInstancingD3D11Percent": "100",
  "FIntEmotesAnimationsPerPlayerCacheSize": "16777216",
  "DFIntStartupTracingInfluxRollout": "0",
  "FFlagEnableSoundTelemetry": "False",
  "FFlagFacialAnimationStreamingServiceUserSettingsOptInVideo": "False",
  "DFIntGoogleAnalyticsLoadPlayerHundredth": "0",
  "DFIntBrowserTrackerApiDeviceInitializeRolloutPercentage": "0",
  "FFlagNullCheckCloudsRendering": "True",
  "FFlagAvatarChatServiceExposeClientFeaturesForVoiceChat": "False",
  "FFlagGraphicsGLEnableSuperHQShadersExclusion": "False",
  "FFlagPreloadTextureItemsOption4": "True",
  "DFStringAnalyticsNS1ApplicationId": "opt-out",
  "DFFlagEphemeralCounterInfluxReportingEnabled": "False",
  "FFlagEnableCameraByDefault": "False",
  "FFlagGpuGeometryManager7": "True",
  "DFIntLoginTelemetryHundredthsPercent": "0",
  "DFFlagClientBaseNetworkMetrics": "False",
  "DFStringAnalyticsNS1BeaconConfig": "https://opt-out.roblox.com",
  "FFlagRenderCheckThreading": "True",
  "FIntPGSAngularDampingPermillPersecond": "9999999999",
  "FIntLightingDefaultClearColorARGB": "True;255,255,255,255",
  "FIntRenderLocalLightFadeInMs_enabled": "99999",
  "FFlagTopBarUseNewBadge": "false",
  "FFlagEnableBetaBadgeLearnMore": "false",
  "FFlagBetaBadgeLearnMoreLinkFormview": "false",
  "FFlagControlBetaBadgeWithGuac": "false",
  "FStringVoiceBetaBadgeLearnMoreLink": "null",
  "DFFlagDebugEnableInterpolationVisualizer": "true",
  "FFlagReconnectDisabled": "True",
  "FFlagEnableInGameMenuChrome": "True",
  "FFlagEnableInGameMenuChromeABTest": "True",
  "FFlagDebugGraphicsDisableVulkan": "True",
  "FFlagDebugGraphicsDisableVulkan11": "True",
  "FFlagDebugForceFutureIsBrightPhase2": "True",
  "DFFlagDebugRenderForceTechnologyVoxel": "True",
  "FFlagMouseLocationUpdateSooner": "True",
  "DFFlagAnimatorEnableNewAdornments": "True",
  "DFIntMaxAcceptableUpdateDelay": "1",
  "FIntActivatedCountTimerMSTouch": "1",
  "DFFlagAllowRegistrationOfAnimationClipInCoreScripts": "True",
  "DFIntReplicatorDataPingReportThrottleSeconds": "5",
  "DFIntHttpBatchApi_maxReqs": "5",
  "DFFlagRakNetDetectRecvThreadOverload": "True",
  "DFIntPerformanceControlFrameTimeMax": "1",
  "DFIntSignalRCoreHubMaxElapsedMs": "20000",
  "FFlagDebugNextGenReplicatorEnabledWriteCFrameColor": "True",
  "DFFlagRakNetUnblockSelectOnShutdownByWritingToSocket": "True",
  "FIntActivatedCountTimerMSMouse": "1",
  "FFlagPackageAnalyticsPlacePublishOptimization": "True",
  "DFIntBufferCompressionLevel": "0",
  "DFIntMaxProcessPacketsJobScaling": "10000",
  "DFFlagAnimatorFixReplicationASANError": "True",
  "FIntRuntimeMaxNumOfMutexes": "1000000",
  "DFIntBatchThumbnailMinWaitMs": "1",
  "FIntRuntimeMaxNumOfSchedulers": "1000000",
  "DFIntWaitOnUpdateNetworkLoopEndedMS": "100",
  "FFlagEnablePerformanceControlService": "True",
  "DFFlagGameNetFixReplicationSkipBug": "True",
  "DFIntSignalRHubConnectionConnectTimeoutMs": "2000",
  "DFIntBatchThumbnailResultsSizeCap": "200",
  "DFFlagRakNetDisconnectNotification": "True",
  "FIntRuntimeMaxNumOfDPCs": "64",
  "DFIntNetworkSchemaCompressionRatio": "100",
  "DFFlagJointIrregularityOptimization": "True",
  "FFlagNextGenReplicatorEnabledWrite": "True",
  "DFIntWaitOnRecvFromLoopEndedMS": "10",
  "DFIntClusterCompressionLevel": "1",
  "FFlagEnableDelayedInputForSetFavorite": "True",
  "DFIntHttpBatchApi_minWaitMs": "1",
  "FIntSmoothClusterTaskQueueMaxParallelTasks": "8",
  "DFIntMaxFrameBufferSize": "4",
  "DFFlagCorrectServerReplicatorStatsIP": "True",
  "DFFlagLuauImproveNonFunctionCallError": "True",
  "DFIntNetworkClusterPacketCacheNumParallelTasks": "8",
  "DFFlagPauseSurfaceControllerBeforeSwappingDataModel2": "True",
  "DFFlagPhysicsMechanismCacheOptimizeAlloc": "True",
  "DFFlagReplicatorCheckReadTableCollisions": "True",
  "DFFlagRakNetDecoupleRecvAndUpdateLoopShutdown": "True",
  "DFIntSignalRCoreHubMaxBackoffMs": "10000",
  "FStringGetPlayerImageDefaultTimeout": "1",
  "FIntSmoothMouseSpringFrequencyTenths": "200",
  "DFFlagClampIncomingReplicationLag": "True",
  "DFFlagSimSmoothedRunningController2": "True",
  "FFlagQuaternionPoseCorrection": "True",
  "DFIntConnectingTimerInterval": "10",
  "DFFlagNextGenRepRollbackOverbudgetPackets": "True",
  "DFIntCodecMaxIncomingPackets": "50",
  "FIntActivatedCountTimerMSKeyboard": "1",
  "FStringRemoteAnimationSmoothingStrategy": "ExponentialDecay",
  "DFIntBufferCompressionThreshold": "100",
  "FFlagOnlyDecrementCompletenessIfReplicating": "True",
  "DFIntSignalRCoreTimerMs": "200",
  "FFlagEnableAnimatorSkipCopyPreviousRigKeyOnJointModification": "True",
  "DFIntBatchThumbnailMaxWaitMs": "3",
  "FFlagUISUseLastFrameTimeInUpdateInputSignal": "True",
  "DFIntBatchThumbnailLimit": "128",
  "FFlagAnimatorRetargetSkipAnkleModification": "True",
  "FIntSimSolverResponsiveness": "2147483647",
  "DFIntBatchPostLimit": "128",
  "DFFlagAcceleratorUpdateOnPropsAndValueTimeChange": "True",
  "FFlagDebugLargeReplicatorWrite": "True",
  "FIntRuntimeMaxNumOfThreads": "1000000",
  "DFIntCodecMaxOutgoingFrames": "10000",
  "FFlagLuaAppLegacyInputSettingRefactor": "True",
  "FFlagPreComputeAcceleratorArrayForSharingTimeCurve": "True",
  "FIntCoordinatorPlannerStepsPerIteration": "8",
  "DFFlagAnimatorRetargetInterpolateFKCorrection": "True",
  "FIntRuntimeMaxNumOfLatches": "1000000",
  "FFlagDebugLargeReplicatorEnabled": "True",
  "FIntRuntimeMaxNumOfSemaphores": "1000000",
  "FIntOverrideISRReplicatorStepBandwidthBytes": "65536",
  "DFIntHttpBatchApi_maxWaitMs": "3",
  "DFStringR15CollisionTypeField": "universeAvatarCollisionType",
  "DFIntLargePacketQueueSizeCutoffMB": "1000",
  "FIntRuntimeMaxNumOfConditions": "1000000",
  "DFFlagReplicatorSeparateVarThresholds": "True",
  "DFFlagSimOptimizeGeometryChangedAssemblies2": "True",
  "FFlagNextGenReplicatorEnabledRead": "True",
  "DFIntSkipSomePropertiesPermyriad": "5000",
  "DFFlagCorrectCachePolicySkipRedirectCache": "True",
  "DFIntHttpBatchApi_cacheDelayMs": "10",
  "DFIntBatchThumbnailMaxReqests": "3",
  "DFFlagRakNetCalculateApplicationFeedback2": "True",
  "DFIntHttpBatchApi_bgDelayMs": "1",
  "DFIntSignalRCoreServerTimeoutMs": "10000",
  "DFIntSignalRCoreHubBaseRetryMs": "100",
  "DFIntMaxDataPacketPerSend": "2147483647",
  "DFIntClientPacketMaxDelayMs": "1",
  "FIntInterpolationMaxDelayMSec": "100",
  "DFIntDataSenderRate": "38760",
  "FFlagMouseGetPartOptimization": "True",
  "DFFlagEnablePerfDataCoreTimersCollection2": "False",
  "FFlagEnableZstdDictionaryForClientSettings": "False",
  "DFFlagReportEphemeralEarlyKeyUsage": "False",
  "FFlagLuaMenuPerfImprovements": "True",
  "FFlagEnableInGameMenuDurationLogger": "False",
  "DFFlagFrameTimeStdDev": "False",
  "DFFlagCreateMeshPartAtRuntime": "False",
  "FFlagPushFrameTimeToHarmony": "True",
  "FFlagProcessEventQueueOnInput": "True",
  "DFIntDownloadEpisodeTimerFreqeuncyInMs": "100",
  "DFIntTimestepArbiterAccelerationModelFactorThou": "50000",
  "DFIntClientPacketExcessMicroseconds": "1000",
  "DFIntPerformanceControlFrameTimeMaxUtility": "-1",
  "DFIntSignalRHubConnectionHeartbeatTimerRateMs": "2000",
  "FFlagDebugCodegenOptSize": "True",
  "DFFlagReportHumanoidRigUpdate": "False",
  "FFlagDebugDisableOptimizedBytecode": "False",
  "DFIntInitialAccelerationLatencyMultTenths": "1",
  "DFFlagDebugRemoteRequestEnableAllTimerGroups": "False",
  "DFFlagCanClientReplicateProp": "False",
  "DFFlagEnablePerfDataSubsystemTimersCollection2": "False",
  "DFIntHttpBatchApi_MaxBatchesSentPerCyle": "10",
  "FFlagKeepZeroInfluenceBones": "False",
  "DFIntReplicatorDataPingReportHundredthPercentage": "0",
  "FFlagUserUpdateInputConnections": "True",
  "DFFlagDebugOverrideDPIScale": "False",
  "DFIntThrottlingPredictionAccelerationHoldThousandth": "2",
  "DFFlagReportHumanoidRigAndModelTypeIfDifferent": "False",
  "FFlagDebugLargeReplicatorRead": "True",
  "FFlagSortKeyOptimization": "True",
  "FFlagEnableRbxPostAPI": "True",
  "FFlagFasterPreciseTime3": "True",
  "DFIntClientPacketMaxFrameMicroseconds": "200",
  "DFFlagMouseMoveOncePerFrame": "False",
  "DFFlagNetworkHumanoidStatePropertyReplicationWarmup": "False",
  "DFIntNetworkQualityResponderMaxWaitTime": "1",
  "FFlagSimEnableDCD16": "True",
  "FFlagImproveShiftLockTransition": "True",
  "DFIntSignalRHubConnectionBaseRetryTimeMs": "100",
  "DFIntMaxReceiveToDeserializeLatencyMilliseconds": "10",
  "DFIntTimeBetweenSendConnectionAttemptsMS": "200",
  "DFIntNetworkInProcessLimitGameplayMsClient": "1",
  "DFIntRCCCheckCoalescedTouchEventualConsistencyInMS": "-1",
  "DFIntMaxProcessPacketsStepsAccumulated": "0",
  "DFIntNetworkQualityResponderUnit": "10000000",
  "DFIntMaxProcessPacketsStepsPerCyclic": "5000",
  "DFIntClientPacketHealthyAllocationPercent": "20",
  "FFlagEnableZstdForClientSettings": "False",
  "DFIntBatchThumbnailMaxExponentialRetries": "2",
  "DFIntMegaReplicatorNetworkQualityProcessorUnit": "10",
  "DFIntGraphicsOptimizationModeMaxFrameTimeTargetMs": "25",
  "DFIntTimestepArbiterAngAccelerationThresholdThou": "2000",
  "DFIntReplicatorJdiReportThrottlePercent": "0",
  "DFIntSignalRCoreHandshakeTimeoutMs": "5000",
  "FFlagSkipJoinedSessionLog": "True",
  "DFIntGraphicsOptimizationModeMinFrameTimeTargetMs": "16",
  "DFFlagEnablePerfDataCoreCategoryTimersCollection2": "False",
  "DFIntReplicatorDataPingReportThresholdMs": "5000",
  "DFIntHttpBatchApi_bgRefreshMaxDelayMs": "5",
  "DFFlagSkipSomePropertiesSkip": "True",
  "DFFlagSolverStateReplicatedOnly2": "True",
  "DFFlagSkipReadDiskCacheRedirects": "True",
  "DFFlagUnifyLegacyJointGeometry": "True",
  "DFFlagAnimatorAnywhere": "True",
  "DFFlagMergeFakeInputEvents3": "True",
  "DFFlagOptimizePartsInPart": "True",
  "DFFlagRakNetDetectNetUnreachable": "True",
  "DFFlagReplicateCreateToPlayer": "True",
  "DFFlagSkipSomeProperties": "True",
  "DFFlagSimOptimizeSetSize": "True",
  "DFFlagRakNetUseSlidingWindow4": "True",
  "DFFlagRakNetEnablePoll": "True",
  "DFFlagOptimizeExtents": "True",
  "DFFlagOptimizeClusterCacheAlloc": "True",
  "DFFlagAllowPropertyDefaultSkip": "True",
  "FFlagMessageBusCallOptimization": "True",
  "DFFlagOptimizeIsA": "True",
  "DFFlagNetworkSchemaImprovements": "True",
  "DFIntSignalRCoreKeepAlivePingPeriodMs": "5000",
  "DFIntReplicationDataCacheNumParallelTasks": "8",
  "DFIntInterpolationNumParallelTasks": "8",
  "DFIntPhysicsReceiveNumParallelTasks": "8",
  "DFIntMegaReplicatorNumParallelTasks": "8",
  "DFIntRuntimeConcurrency": "8",
  "FIntFullscreenTitleBarTriggerDelayMillis": "3600000",
  "TextureQualityOverrideEnabled": "True",
  "DebugPauseVoxelizer": "True",
  "DebugPerfMode": "True",
  "LocalLightCountsInCompatibilityThrottlePerTenThousand": "0",
  "DebugDisplayFPS": "False",
  "TaskSchedulerLimitTargetFpsTo2402": "False",
  "TaskSchedulerTargetFps": "9999",
  "ExperienceStateCaptureHighlightTransparencyPercent": "0",
  "CSGLevelOfDetailSwitchingDistanceL34": "0",
  "CSGLevelOfDetailSwitchingDistanceL12": "0",
  "TreeDiffModCheckShadowReportingRate": "0",
  "CSGLevelOfDetailSwitchingDistance": "0",
  "LightgridAsyncChunkContextCount": "0",
  "DebugFRMQualityLevelOverride": "1",
  "TextureQualityOverride": "3",
  "RenderShadowHugeRadius": "0",
  "LightstepHTTPTransportUrlPath": "null",
  "LightstepHTTPTransportUrlHost": "null",
  "LightstepToken": "null",
  "HandleAltEnterFullscreenManually": "False",
  "DebugForceFSMCPULightCulling": "False",
  "DebugLightgridCPUForceSync": "False",
  "RenderInitShadowmaps": "False",
  "FastGPULightCulling3": "True",
  "NewLightAttenuation3": "True",
  "RenderCBRefactor2": "True",
  "DebugSSAOForce": "False",
  "DisablePostFx": "True",
  "DebugSkyGray": "True",
  "RenderMaxShadowAtlasUsageBeforeDownscale": "0",
  "RenderShadowMapDepthCacheMinNodes": "0",
  "RenderShadowMapDepthCacheMemLimit": "0",
  "DebugFRMOptionalMSAALevelOverride": "1",
  "GrassMovementReducedMotionFactor": "0",
  "DebugTextureManagerSkipMips": "7",
  "RenderLocalLightUpdatesMin": "0",
  "RenderLocalLightUpdatesMax": "0",
  "UnifiedLightingBlendZone": "0",
  "RenderSurfaceLightOffset": "0",
  "RenderLocalLightFadeInMs": "0",
  "DebugForceMSAASamples": "1",
  "FRMMaxGrassDistance": "0",
  "RenderShadowmapBias": "0",
  "FRMMinGrassDistance": "0",
  "RenderUseTextureManager224": "False",
  "TM2SkipMipsForUnstreamable2": "True",
  "DoNotSkipMipsBasedOnSystemMemoryPS": "True",
  "DebugLimitMinTextureResolutionWhenSkipMips": "9999999",
  "EnablePowerTraceModule": "True",
  "IncludePowerSaverMode": "True",
  "BloomFrmCutoff": "1",
  "SSAOMipLevels": "0",
  "FFlagMSRefactor5": "False",
  "FFlagEnableInGameMenuChromeABTest3": "False",
  "FIntDebugTextureManagerSkipMips": "7",
  "FIntCameraFarZPlane": "500"
}
```
