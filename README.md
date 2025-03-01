# Laptop Setup

## Gear

- MSI Vector 16 HX (i7-14700HX + RTX 4080 175W)

- LG UltraGear 27GR83Q-B @ 240Hz

- Durgod Taurus K310 (Cherry MX Red)

- Endgame Gear XM2 8K @ 800 DPI, 1000 Hz

## BIOS

- Unlock overclocking
- Unlock undervolting
- Unlock CFG
- Disable hyperthreading

## Windows 11

- Install Windows -> Time and currency format -> English (World)

- Install Windows updates -> reboot -> repeat

- Use ChrisTitus Windows 11 tool to optimize stuff (Run PowerShell as admin):
  
      iwr -useb https://christitus.com/win | iex

- Uninstall NVidia driver with `Display Driver Uninstaller` if there's any

- Install NVidia driver with `NVCleanstall`

- Install monitor driver

- Enable HDR

- Install `ThrottleStop`

- Install `MSI Afterburner` + `RivaTuner Statistics Server`

- Install `Custom Resolution Utility`

- Mouse -> Enhance pointer precision: off

## ThrottleStop

- Check CPU microcode version and apply 0x12B or newer if exists

- FIVR -> P Cores @ 3.5 GHz, E Cores @ 3.0 GHz, -125mV

- TPL -> Long power ON [55W, Clamp], Short power ON [66W, Clamp]

## MSI Afterburner

- 2400MHz @ 875mV

## Custom Resolution Utility

- Set VRR range to 1-240Hz

## NVidia Control Panel

`Adjust image settings with preview`

1. Apply performance preset

2. Use the advanced 3D image settings

3. Click "take me there""

`Manage 3D Settings`

- Low latency mode: Ultra

- Monitor Technology: G-Sync

- Vertical sync: On

- Background frame rate: 30 FPS

- Power management: Prefer maximum performance

- Texture filtering quality: High performance

`Change resolution`

- Use nvidia color settings
  
  - 12bpc

`Adjust desktop color settings`

- Digital vibrance (if HDR is washed): 55-60%

`Set up digital audio`

- HDMI: Turn off audio

`Adjust desktop size and composition`

- Scaling mode: Full screen

`Set up G-SYNC`

* Enable G-Sync, G-Sync compatible: ON
* Enable for full screen mode
* Select monitor -> Enable settings for the selected display model

## Steam

- Run as administrator

## In-game

- (Exclusive) Fullscreen

- Max frame rate: unlimited (or highest possible)

- V-Sync: OFF

- NVidia Reflex: ON + BOOST

## Crucial information for competitive FPS gamers

As a rule of thumb, turn down all the graphics settings ingame to maximize performance.

Monitor your GPU core clock while playing.

If your GPU core clock drops down from the maximum value, turn your game graphics settings UP in little steps until it's stable.
