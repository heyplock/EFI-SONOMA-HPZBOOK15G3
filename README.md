# EFI-SONOMA-HPZBOOK15G3
- Opencore EFI Folder for Hp Zbook 15 G3 with Hakintosh Sonoma 14.6
- !! USE AT YOUR OWN RISK - IM NOT A PROFESSIONNAL - YOU CAN GET YOUR APPLE ID LOCKED IF YOU DO NOT INSTALL IT CORRECTLY THEN SIGN IN !! 
- Please read and understand [dortiana's guide here]() before using these

  ![](/EFI-SONOMA-HPZBOOK15G3/Screenshots/Sonoma.png?raw=true "")

# REPOSITORY CONTENT

- EFI Folder
- Readme.md
- Screenshots
  
# PREREQUIES

## I - HARDWARE I USED
  - CPU : Intel Core i7-6700HQ
  - iGPU : Intel HD 530 (Nvidia card disabled in BIOS settings)
  - RAM : 16Gb DDR4 2133Mhz
  - SSD : Some random 500Gb NVME
  - Screen : 15,6" 1920x1080
  - More info [here](https://support.hp.com/ca-fr/document/c04956278) (FR)
    
## II - BIOS SETUP
  - Secure boot : off
  - Legacy Support : off
  - Fastboot : off
  - PXE boot : off
  - W.O.L ( wake on LAN ) : off
  - Wake on USB : off
  - Deep Sleep : off
  - LAN/WAN Auto switching : off
  - Graphics mode : Auto
  - Memory size : 64Mb
  - Fingerprint : off
  - Extended Idle Power States : off

  Leave everything else at default state
  
## III - TOOLS NEEDED

- [OpencorePKG]() for /macrecovery (please check [dortiana's guide here]() )
- [ProperTree]() for editing your config.plist and set your own SMBIOS values
- [GenSMBIOS]() for generating SMBIOS values
- USB Stick (+4gb)
- Python3 or newer

# IV WHAT'S WORKING

- WiFi (using [Heliport]() app)
- Bright
- Function buttons for brightness & sound
- Graphics acceleration
- Battery status
- iServices ( iMessages issues fixed with itlwn.kext and Heliport )
- Bluetooth
- Sleeping issues fixed in my case

# V - How to use 

- Use Disk manager or Rufus to make your USB stick ready to go ( Check [dortiana's guide]() )
- Drag "EFI" folder to the root ( / ) of your USB stick
- Generate your recovery files with OpencorePKG 

- copy the folder that's been generated to the root of your USB stick
- open ProperTree and GenSMBIOS
- Genrate values for MacBookPro15,2 and copy them into your config.plist using ProperTree ( Again, check [dortiana's guide here]() if needed )
- Boot from USB Stick and select "YOURUSB(dmg)"
- Install MacOS Sonnoma

# VI - ISSUES I ENCOUNTERED 

- For WiFi support, please install and use [Heliport]()


