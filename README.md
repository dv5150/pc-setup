# Laptop Setup

## Gear

- MSI Vector 16 HX (i7-14700HX + RTX 4080 175W)

- LG UltraGear 27GR83Q-B @ 240Hz

- Durgod Taurus K310 (Cherry MX2A Silent Red)

- Zowie FK2-C @ 800 DPI, 1000 Hz

## BIOS

- Enabling undervolting:
  - Unlock overclocking
  - Unlock undervolting
  - Unlock CFG

- Fixing PCH temperature
  - Reduce DMI Link Speed to slowest possible value
  - Set PCI Express Root Port #1 and #3 speed to Gen 1
  - Set PCI Express Root Port #2 speed to Gen 3
  - Set all other enabled PCI Express ports' speed to Gen 2

## Windows 11

- Install Windows -> Time and currency format -> English (World)

- Install Windows updates -> reboot -> repeat

- Disable `Memory Integrity`, `Kernel-mode Hardware-enforced Stack Protection`, `Local Security Authority Protection` and `Microsoft Vulnerable Driver Blocklist`

- Use ChrisTitus Windows 11 tool to optimize stuff (Run PowerShell as admin):
  
      iwr -useb https://christitus.com/win | iex

- Uninstall NVidia driver with `Display Driver Uninstaller` if there's any

- Install NVidia driver with `NVCleanstall`

- Install `ThrottleStop`

- Install `MSI Afterburner` + `RivaTuner Statistics Server`

- Install `Revo Uninstaller`

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

- Max frame rate: Off

- Power management: Normal

- Texture filtering quality: High performance

## Steam

- Run as administrator

## In-game

- (Exclusive) Fullscreen

- Max frame rate: unlimited (or highest possible)

- V-Sync: OFF

- NVidia Reflex: ON + BOOST

## Fix Reaper audio crackling when in background:

- `powercfg /powerthrottling disable /path "C:\Program Files\REAPER (x64)\reaper.exe"`
- `powercfg /powerthrottling disable /path "C:\Program Files\Arobas Music\Guitar Pro 8\GuitarPro.exe"`
- Use ProcessLasso to set CPU affinity (4 cores) and High I/O priority on Reaper and Guitar Pro
- Unpark CPU cores
