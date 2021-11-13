# How to cook Manjaro Gnome on MateBook X Pro 2021 

## MateBook X Pro 2021 Spec
<pre>
<font color="#3465A4"><b>Type:</b></font> Laptop <font color="#3465A4"><b>System:</b></font> HUAWEI <font color="#3465A4"><b>product:</b></font> MACHD-WXX9
<font color="#3465A4"><b>CPU</b> <font color="#3465A4"><b>Info:</b></font> Quad Core <font color="#3465A4"><b>model:</b></font> 11th Gen Intel Core i7-1165G7
<font color="#3465A4"><b>Graphics:</b></font> Intel TigerLake-LP GT2 [Iris Xe Graphics]
<font color="#3465A4"><b>Webcamera</b></font> kingcome HD Camera
<font color="#3465A4"><b>Audio:</b></font> Intel Tiger Lake-LP Smart Sound Audio
<font color="#3465A4"><b>Network:</b></font> Intel Wi-Fi 6 AX201
<font color="#3465A4"><b>Bluetooth:</b></font> Intel AX201 Bluetooth
</pre>

## What's Good (out of the box)
- Touchpad and gestures
- Wi-Fi
- Bluetooth
- FN keys
- Webcamera
- Mic
- Hibernation

## What's Bad (out of the box)
- Video tearings and freezes, especialy on Wayland (see hot to fix below)
- Audio system doesn't works at all (see hot to fix below)
- Fingerprint sensor doesn't works (still no drivers)

## Installation
**Disabling Secure Boot**
- Press F2 on boot stage
- Disable "Secure boot"
- Save and Exit

**Booting to Installer**
- Press F12 on boot stage
- Select USB flash with Manjaro

**Installing Manjaro**
- Select "Boot"
- Press "E" for edit booting params
- Add to the end of "LINUX" string:

`i915.enable_psr=0`

- Ctrl+X to boot, install Manjaro and reboot

**Manjaro First Run**
- When GRUB show, select "Advanced Params"
- Press "E" for edit booting params
- Add to the end of "LINUX" string:

`i915.enable_psr=0`

- Ctrl+X to boot

## Fixes
**Video**
- Edit boot params:

`sudo nano /etc/default/grub`

- Add "i915.enable_psr=0" to the end of LINUX strings:

`GRUB_CMDLINE_LINUX_DEFAULT="quiet splash apparmor=1 security=apparmor udev.log_priority=3 i915.enable_psr=0"
 GRUB_CMDLINE_LINUX="i915.enable_psr=0"`

- Save and exit
- Update GRUB:

`sudo update-grub`

**Audio**
- Check for hardware errors:

`sudo dmesg | grep audio`

- Find suggestion to try SOF driver and link to the https://github.com/thesofproject/sof-bin
- Download latest release and install it:

`cd <sof-bin-archive>`
`./install.sh <version>` ex. `./install.sh v1.9` 

- Reboot 
- Check that audio works

## Still Broken
- Fingerprint sensor still doesn't works cause no drivers for it


