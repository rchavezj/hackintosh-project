## EDO'S HACKINTOSH PROJECT

#### 0. INTRO

This guide is a log of the steps I've taken to put my system running OSX Catalina 10.15.3.

DISCLAIMER: *Follow this guide at your own responsibilty. I'm not responsible for any damage  you commit to your hardware*

If you try to just copy/paste the thing, you won't have any luck. First there are personal files that need to be created from your target hardware. Other is because each system has its own differences. So if you're trying to do this the fast way, my advice to you is just buy a new Mac from Apple.

I've followed the AMD OS X Vanilla Guide [here](https://vanilla.amd-osx.com)

I have no credits for this, besides this document that can help you a lot if your hardware is same as mine.

All credits to the guys at AMD OS X Vanilla Guide :heart

So the purpose here is to create an hackintosh from Catalina 10.15.3 with OpenCore bootloader.


#### 1. HARDWARE

List of the hardware I'm using:

    - Case Extended ATX NZXT Ht700i w/Black Window
    - Power Supply: NZXT E650 Digital 650W 80 PLUS Gold Full Modular Black
    - AMD Ryzen 9 3900X 12-Core 3.8 GHz Turbo 4.6GHz 70MB Socket AM4
    - CPU Water Cooler NZXT Kraken X52 v2
    - Motherboard ATX Gigabyte X570 Aorus Master
    - RAM GSkill Trident Z RGB (for AMD) 4x16GB DDR-4-3200MHz CL16 Black
    - Graphics Card RADEON RX5700 XT 8GB
    - 2x SSD M.2 2280 Samsung 970 Evo Plus 500GB
    - Razer Seiren X Condenser Streaming Microphone
    - Razer Kiyo FHD Webcam
    - Mouse Logitech G-903
    - Keyboard Ducky MECHA MINI 60%

#### 2. THINGS YOU'LL NEED

    - PEN DRIVE 16GB
    - XCode installed
    - A macOS Catalina 10.15.3 install (Install macOS Catalina.app)
        NOTE: download it directly from the App Store using your own account
    - iCloud account (usually people already have one)
    - lots of patience
    - lots of google-fu


#### 3. GATHERING RESOURCES

Things you'll need to download before starting:

OpenCore-0.5.5
GenSMBIOS
MasciASL-1.5.7
MountEFI
ProperTree
SSDTTime
The Vanilla AMD config courtesy of AlGrei [The Vanilla AMD config courtesy of AlGrei](https://github.com/AMD-OSX/AMD_Vanilla)

#### 4. INSTALLATION

    macOS

    Create an USB with Catalina 10.15.3 install

    1. Download Catalina from App Store

    2. Format your USB with
       - Name: Hackintosh
       - Format: APFS
       - Scheme: GUID Partition Map

    3. Run  the createinstallmedia command

    ```
        sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/Hackintosh
    ```

    This will take some time but in the end you'll have a normal Catalina USB installer.

    Nothing new till now.



#### 4. CREATING MACOS INSTALL USB AND BOOTLOADER SETUP

    1. Run MakeInstall as Admin from within the gibMacOS folder.

    2. Select your USB drive number. If you choose to use OpenCore add an O to the number: i.e. 4O
    I've chosen OpenCore as it is advised from OSX 10.15.2 onwards.

#### 5. KEXT


#### 10. PREPARE YOUR BIOS FOR HACKINTOSH (GIGABTE AORUS MASTER)


    1. UPDATE BIOS TO THE LATEST ONE (not always the best, but in most cases it is...)

    2. LOAD OPTIMIZED DEFAULT

    OC Features

    3. EXTREME MEMORY PROFILE (X.M.P): set it to Profile 1

    BIOS

    4. FAST BOOT: disabled

    5. Windows 8/10 Features: set to Windows 8/10

    6. CSM Support: Enabled, if you have problems disable it

    7. LAN PXE Boot Option ROM: set to disabled

    8. Storage Boot Option Control: UEFI

    9. Other PCI Devices: UEFI

    PERIPHERALS

    10. PCIe 1 Slot

    11. Security Device Support: Disabled

    12. USB Configuration

        - XHCI Hando-off: Enabled

        - Legacy USB Support: Enabled

    13. Network Stack: Disabled

    14. SATA Mode: AHCI

    CHIPSET

    15. VT-d: Enabled

    16. Internal Graphics: Enabled (even if you have dedicated GPU)

    17. IOAPIC 24-119 Entries: Enabled

    POWER

    18. Platform Power Management: Disabled


#### 15. LINK SECTION

[The Vanilla AMD config courtesy of AlGrei (check the link section)


        - A USB Drive (16GB)
        - Some patience... lots of it... more of it...

        Keep calm, with this quick guide you'll do it almost without a struggle :heart

#### 3. INSTALLATION

    macOS

    Create an USB with Catalina 10.15.3 install

    1. Download Catalina from App Store

    2. Format your USB with
       - Name: Hackintosh
       - Format: APFS
       - Scheme: GUID Partition Map

    3. Run  the createinstallmedia command

    ```
        sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/Hackintosh
    ```

    This will take some time but in the end you'll have a normal Catalina USB installer.

    Nothing new till now.



#### 4. CREATING MACOS INSTALL USB AND BOOTLOADER SETUP

    1. Run MakeInstall as Admin from within the gibMacOS folder.

    2. Select your USB drive number. If you choose to use OpenCore add an O to the number: i.e. 4O
    I've chosen OpenCore as it is advised from OSX 10.15.2 onwards.

#### 5. KEXT


#### 10. PREPARE YOUR BIOS FOR HACKINTOSH (GIGABTE AORUS MASTER)


    1. UPDATE BIOS TO THE LATEST ONE (not always the best, but in most cases it is...)

    2. LOAD OPTIMIZED DEFAULT

    OC Features

    3. EXTREME MEMORY PROFILE (X.M.P): set it to Profile 1

    BIOS

    4. FAST BOOT: disabled

    5. Windows 8/10 Features: set to Windows 8/10

    6. CSM Support: Enabled, if you have problems disable it

    7. LAN PXE Boot Option ROM: set to disabled

    8. Storage Boot Option Control: UEFI

    9. Other PCI Devices: UEFI

    PERIPHERALS

    10. PCIe 1 Slot

    11. Security Device Support: Disabled

    12. USB Configuration

        - XHCI Hando-off: Enabled

        - Legacy USB Support: Enabled

    13. Network Stack: Disabled

    14. SATA Mode: AHCI

    CHIPSET

    15. VT-d: Enabled

    16. Internal Graphics: Enabled (even if you have dedicated GPU)

    17. IOAPIC 24-119 Entries: Enabled

    POWER

    18. Platform Power Management: Disabled


#### 15. LINK SECTION
