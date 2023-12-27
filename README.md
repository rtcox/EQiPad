# EQiPad
Stream Everquest to an iPad or  mobile device to play with a controller

![screenshot](https://i.imgur.com/OnaUib7.png)
![inuse](https://i.imgur.com/EXuVnNU.jpg)
![handheld](https://i.imgur.com/aulIV6v.jpg)

## Requirements
### Hardware Requirements:
- PC or Laptop to stream from
   - I recommend a dedicated computer for this with a hardwired LAN connection: An old laptop, etc. Otherwise you will have audio and resolution issues you’ll need to adjust each time before and after you stream.
- iPad or Tablet
- Bluetooth Game Controller
- Bluetooth Keyboard (or XBOX Gamepad {untested})
#### To use a laptop in a closed-lid mode or PC without an attached monitor: 
- Dummy Plug: https://www.amazon.com/dp/B06XT1Z9TF?psc=1&ref=ppx_yo2ov_dt_b_product_details
### Software Requirements:
#### Streaming PC:
- Sunshine: https://github.com/LizardByte/Sunshine/releases/tag/v0.21.0
- Controller Companion: https://store.steampowered.com/app/367670/Controller_Companion/
- Custom Resolution Utility: https://www.monitortests.com/forum/Thread-Custom-Resolution-Utility-CRU
- ViGEmBus: https://github.com/nefarius/ViGEmBus
#### Tablet/Phone:
- Moonlight: https://moonlight-stream.org/
#### UI:
- https://github.com/rtcox/EQiPad
## Setup:
### Step 1: Configure OS Resolution
- Identify native tablet/phone resolution (look it up on Google)
  - Ex. The iPad Air 5 has a native resolution of 2360x1640
- Halve the resolution for High DPI screens. Else the UI will be unusable for touch and mouse
  - **1180x820**
- Download and run Custom Resolution Utility
- Add into the list the determined resolution
![CRU](https://i.imgur.com/IOXRWiz.png)
- Windows: Open Display Settings and apply the new resolution
![Displaysetting](https://i.imgur.com/Efw1QE3.png)
- Windows: Adjust Power Options to never turn off the screen, hibernate or go to sleep 
#### For closed-lid laptops or desktops with no monitor only: 
- Laptop only: Set lid close action to Do Nothing
  - https://www.tenforums.com/tutorials/69762-how-change-default-lid-close-action-windows-10-a.html
- Install Dummy Plug and set screens to mirrored mode
  -	https://support.microsoft.com/en-us/windows/screen-mirroring-and-projecting-to-your-pc-5af9f371-c704-1c7f-8f0d-fa607551d09c
### Step 2: Configure EQ Client
-	Open eqclient.ini from the Everquest game directory in a text editor and adjust the lines to match your screen resolution
```
WindowedMode=FALSE
[VideoMode]
BitsPerPixel=32
Width=1180
Height=820
WidthWindowed=1180
HeightWindowed=820
WindowedWidth=1180
WindowedHeight=820
RefreshRate=99
```
•	Extract iPadUI.zip to \<Everquest Install Directory\>\uifiles\iPadUI
### Step 3: Configure PC Utilities
- Install and configure Sunshine https://docs.lizardbyte.dev/projects/sunshine/en/latest/about/installation.html
  - I just use Desktop mode, but you can configure eqgame.exe as another launch option
- Install ViGEmBus
- Install Controller Companion
- Configure Controller Companion profile
  - Examples in Appendix
- Verify Sunshine and Controller Companion are set to launch at startup
### Step 4: Configure Tablet
- Pair game controller and keyboard to tablet/phone
- Install Moonlight
- Configure Custom resolution to native device resolution
  - ex. iPad Air 5: **2360x1640**
### Step 5: Test
- Open Moonlight and connect to host
- Choose Desktop Mode
- Test gamepad functionality: https://hardwaretester.com/gamepad
### Step 6: Play!
- Adjust mouse sensitivity settings in game
- ENJOY!

## Appendix
### Controller Companion Sample Config
![CC](https://i.imgur.com/oHKj8Hl.png)
![CC](https://i.imgur.com/QPazJzI.png)
![CC](https://i.imgur.com/SiUGQYu.png)
![CC](https://i.imgur.com/rTULtU6.png)
![CC](https://i.imgur.com/NyrbYat.png)
![CC](https://i.imgur.com/G5pdrgg.png)
