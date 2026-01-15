# Getting VR working on an AMD eGPU (OCuLink) setup
## Overview
This guide documents the only configuration that worked for me
to run VR on an AMD iGPU + AMD eGPU setup using OCuLink.

This is a niche and fragile setup and should be considered a
last-resort solution.
## My hardware
Thinkpad E14 gen 2 AMD

Ryzen 5 4600u

24 gb

oculink egpu rx 6700 xt

Samsung Odyssey + WMR headset
## Installation

1. Install Windows 10 22H2  
   - Windows 11 may work, but was not tested personally

2. Disable Windows Update  
   - Prevents driver overwrites

3. Install AMD graphics driver **22.11.2**  
   - Newer versions did not work for me

4. Install Windows Mixed Reality Portal  
   - Complete initial headset setup

5. Install Steam, SteamVR, and Mixed Reality for SteamVR  
   - Set SteamVR as the default OpenXR runtime(is optional, some games won't work without it)

### ⚠️ Important notes
- Do **not** use Oasis — it did not work in my setup
- Do **not** use the internal laptop display
- Use an external display (DisplayPort recommended)
## Limitations
- Did not work on newer Windows versions
- Did not work on Linux
- Very sensitive to driver and display configuration
- Not suitable for production or frequent OS updates

Good luck
