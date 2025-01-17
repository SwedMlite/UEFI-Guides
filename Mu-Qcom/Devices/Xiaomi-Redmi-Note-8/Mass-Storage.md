# Enabling Mass Storage

## Description

This Guide will show you how to enable Mass Storage in OrangeFox for Xiaomi Redmi Note 8/8T.

<table>
<tr><th>Table of Contents</th></th>
<tr><td>
  
- Enabling Mass Storage
   - [What's needed](https://github.com/Robotix22/UEFI-Guides/blob/main/Mu-Qcom/Devices/Xiaomi-Redmi-Note-8/Mass-Storage.md#things-you-need)
   - [Preparing](https://github.com/Robotix22/UEFI-Guides/blob/main/Mu-Qcom/Devices/Xiaomi-Redmi-Note-8/Mass-Storage.md#preparing-step-1)
   - [Enable](https://github.com/Robotix22/UEFI-Guides/blob/main/Mu-Qcom/Devices/Xiaomi-Redmi-Note-8/Mass-Storage.md#enable-mass-storage-step-2)

</td></tr> </table>

## Things you need:
   - PC / Laptop
   - [OrangeFox](https://orangefox.download/device/ginkgo)
   - Unlocked Bootloader
   - Modded [msc.sh](https://github.com/Robotix22/UEFI-Guides/blob/main/Mu-Qcom/Devices/Xiaomi-Redmi-Note-8/msc.sh) script

## Preparing (Step 1)

Okay, First you need to boot into the Custom Recovery (OrangeFox) and then enable MTP if disabled (Mount -> Enable MTP). <br />
Then download the msc.sh script and push it to your Device, For Example to `/cache/`: <br />
```
adb push <Path to msc.sh> /cache/
```

## Enable (Step 2)

After you pushed msc.sh to `/cache/` make it executeable and run it **only once**:
```
adb shell
chmod 755 /cache/msc.sh
./cache/msc.sh
```
There will be some errors in output but that dosen't break anything. <br />
On your PC or Laptop should now show up all the partitions of your Phone from LUN 0.
