# Laptop Setup

## Gear

- MSI Vector 16 HX (i7-14700HX + RTX 4080 175W)

- LG UltraGear 27GR83Q-B @ 240Hz

- Durgod Taurus K310 (Cherry MX2A Silent Red)

- Zowie FK2-C @ 800 DPI, 1000 Hz

## BIOS

- Unlock overclocking
- Unlock undervolting
- Unlock CFG
- Disable hyperthreading
- Set PCIe and DMI ASPM values everywhere to L0sL1 if possible, otherwise set to L1
- Reduce DMI Link Speed everywhere [ASUS example](https://10pcg.com/what-is-aspm-in-bios/)

## Windows 11

- Install Windows -> Time and currency format -> English (World)

- Install Windows updates -> reboot -> repeat

- Use ChrisTitus Windows 11 tool to optimize stuff (Run PowerShell as admin):
  
      iwr -useb https://christitus.com/win | iex

- Uninstall NVidia driver with `Display Driver Uninstaller` if there's any

- Install NVidia driver with `NVCleanstall`

- Install `ThrottleStop`

- Install `MSI Afterburner` + `RivaTuner Statistics Server`

## ThrottleStop

- FIVR
  
  - P Cores @ 4.0 GHz
  
  - E Cores @ 3.0 GHz

  - Undervolt [ CPU Core / CPU P Cache / CPU E Cache ] @ -139.6 mV
 
  - Undervolt [ Intel GPU ] @ -49.8 mV
 
  - Undervolt [ System Agent ] @ -40.0 mV

  - CPU Core IccMax @ 215.00 A
 
  - CPU P Cache - Cache Ratio: 40

  - Cache Ratio: Min 35 / Max 40

- TPL
  
  - Long power 45W Clamp
  
  - Short power 45W Clamp

## MSI Afterburner

- 2100MHz @ 825mV

## RivaTuner Statistics Server

- Limit frame rate: 240 FPS

## NVidia Control Panel

`Adjust image settings with preview`

1. Apply performance preset

2. Use the advanced 3D image settings

3. Click "take me there""

`Manage 3D Settings`

- Low latency mode: Ultra

- Monitor Technology: Fixed Refresh

- Vertical sync: Off

- Background frame rate: 30 FPS

- Max frame rate: Unlimited

- Power management: Normal

- Texture filtering quality: High performance

`Change resolution`

- Use nvidia color settings
  
  - 12bpc

## Steam

- Run as administrator

## In-game

- (Exclusive) Fullscreen

- Max frame rate: unlimited (or highest possible)

- V-Sync: OFF

- NVidia Reflex: ON + BOOST
