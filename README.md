# How to cook Manjaro on MateBook X Pro 2021 

## Final Overview
<pre><font color="#4E9A06"><b>██████████████████  ████████</b></font>   <font color="#4E9A06"><b>alardus</b></font>@<font color="#4E9A06"><b>matebook</b></font> 
<font color="#4E9A06"><b>██████████████████  ████████</b></font>   ---------------- 
<font color="#4E9A06"><b>██████████████████  ████████</b></font>   <font color="#4E9A06"><b>OS</b></font>: Manjaro Linux x86_64 
<font color="#4E9A06"><b>██████████████████  ████████</b></font>   <font color="#4E9A06"><b>Host</b></font>: MACHD-WXX9 M1090 
<font color="#4E9A06"><b>████████            ████████</b></font>   <font color="#4E9A06"><b>Kernel</b></font>: 5.13.19-2-MANJARO 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>Uptime</b></font>: 3 hours, 42 mins 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>Packages</b></font>: 1191 (pacman) 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>Shell</b></font>: zsh 5.8 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>Resolution</b></font>: 3000x2000 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>DE</b></font>: GNOME 40.5 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>WM</b></font>: Mutter 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>WM Theme</b></font>: Adwaita-maia-dark 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>Theme</b></font>: Adwaita-maia-dark [GTK2/3] 
<font color="#4E9A06"><b>████████  ████████  ████████</b></font>   <font color="#4E9A06"><b>Icons</b></font>: Adwaita [GTK2/3] 
                               <font color="#4E9A06"><b>Terminal</b></font>: gnome-terminal 
                               <font color="#4E9A06"><b>CPU</b></font>: 11th Gen Intel i7-1165G7 (8) @ 4.700GHz 
                               <font color="#4E9A06"><b>GPU</b></font>: Intel TigerLake-LP GT2 [Iris Xe Graphics] 
                               <font color="#4E9A06"><b>Memory</b></font>: 7216MiB / 15786MiB 

                               <span style="background-color:#2E3436"><font color="#2E3436">   </font></span><span style="background-color:#CC0000"><font color="#CC0000">   </font></span><span style="background-color:#4E9A06"><font color="#4E9A06">   </font></span><span style="background-color:#C4A000"><font color="#C4A000">   </font></span><span style="background-color:#3465A4"><font color="#3465A4">   </font></span><span style="background-color:#75507B"><font color="#75507B">   </font></span><span style="background-color:#06989A"><font color="#06989A">   </font></span><span style="background-color:#D3D7CF"><font color="#D3D7CF">   </font></span>
                               <span style="background-color:#555753"><font color="#555753">   </font></span><span style="background-color:#EF2929"><font color="#EF2929">   </font></span><span style="background-color:#8AE234"><font color="#8AE234">   </font></span><span style="background-color:#FCE94F"><font color="#FCE94F">   </font></span><span style="background-color:#729FCF"><font color="#729FCF">   </font></span><span style="background-color:#AD7FA8"><font color="#AD7FA8">   </font></span><span style="background-color:#34E2E2"><font color="#34E2E2">   </font></span><span style="background-color:#EEEEEC"><font color="#EEEEEC">   </font></span>
</pre>

<pre>
<font color="#3465A4"><b>Graphics:  Device-1:</b></font> Intel TigerLake-LP GT2 [Iris Xe Graphics] <font color="#3465A4"><b>driver:</b></font> i915 <font color="#3465A4"><b>v:</b></font> kernel
           <font color="#3465A4"><b>Device-2:</b></font> kingcome HD Camera <font color="#3465A4"><b>type:</b></font> USB <font color="#3465A4"><b>driver:</b></font> uvcvideo
           <font color="#3465A4"><b>Display:</b></font> <font color="#3465A4"><b>server:</b></font> X.org 1.20.13 <font color="#3465A4"><b>driver:</b></font> <font color="#3465A4"><b>loaded:</b></font> i915 <font color="#3465A4"><b>note:</b></font> n/a (using device driver)
           <font color="#3465A4"><b>resolution:</b></font> &lt;missing: xdpyinfo&gt;
           <font color="#3465A4"><b>OpenGL:</b></font> <font color="#3465A4"><b>renderer:</b></font> Mesa Intel Xe Graphics (TGL GT2) <font color="#3465A4"><b>v:</b></font> 4.6 Mesa 21.2.3
</pre>

## MateBook X Pro 2021 Spec
<pre>
<font color="#3465A4"><b>Type:</b></font> Laptop <font color="#3465A4"><b>System:</b></font> HUAWEI <font color="#3465A4"><b>product:</b></font> MACHD-WXX9
<font color="#3465A4"><b>CPU</b> <font color="#3465A4"><b>Info:</b></font> Quad Core <font color="#3465A4"><b>model:</b></font> 11th Gen Intel Core i7-1165G7
<font color="#3465A4"><b>Graphics:</b></font> Intel TigerLake-LP GT2 [Iris Xe Graphics]
<font color="#3465A4"><b>Webcamera</b></font> kingcome HD Camera
<font color="#3465A4"><b>Audio:</b></font> Intel Tiger Lake-LP Smart Sound Audio
<font color="#3465A4"><b>Network:</b></font> Intel Wi-Fi 6 AX201
<font color="#3465A4"><b>Bluetooth:</b></font> Intel AX201 Bluetooth
<font color="#3465A4"><b>Fingerprint Scanner:</b></font> Goodix GXFP5187
</pre>

## What's Good (out of the box)
- Touchpad and gestures
- Tochscreen
- Wi-Fi
- Bluetooth
- FN keys
- Camera
- Mic
- Hibernation

## What's Bad (out of the box)
- Video tearings and freezes, especialy on Wayland (Intel Iris Xe, see hot to fix below)
- Audio system doesn't works at all (Intel Tiger Lake, see hot to fix below)
- Poor audio quality because only 2 of 4 dynamics are works (here is the fix for 2020 model but still not works for my 2021 lineup, https://github.com/samuelmatn/guides/blob/main/manjaro-matebook.md#set-up-40-surround-speakers)
- Fingerprint sensor doesn't works (Goodix GXFP5187 still has no drivers, https://gitlab.freedesktop.org/libfprint/libfprint/-/issues/112)

## Installation
### Disabling Secure Boot
- Press F2 on boot stage
- Disable "Secure boot"
- Save and Exit

### Booting to Installer
- Press F12 on boot stage
- Select USB flash with Manjaro

### Installing Manjaro
- Select "Boot"
- Press "E" for edit booting params
- Add to the end of "LINUX" string:

`i915.enable_psr=0`

- Ctrl+X to boot, install Manjaro and reboot

### Manjaro First Run
- When GRUB shows, select "Advanced Params"
- Press "E" for edit booting params
- Add to the end of "LINUX" string:

`i915.enable_psr=0`

- Ctrl+X to boot

## Fixes
### Video
- Edit boot params:

`sudo nano /etc/default/grub`

- Add "i915.enable_psr=0" to the end of LINUX strings, eg.:

`GRUB_CMDLINE_LINUX_DEFAULT="quiet splash apparmor=1 security=apparmor udev.log_priority=3 i915.enable_psr=0"`

`GRUB_CMDLINE_LINUX="i915.enable_psr=0"`

- Save and exit
- Update GRUB:

`sudo update-grub`

### Audio
- Check for hardware errors:

`sudo dmesg | grep audio`

- Find suggestion to try SOF driver and link to the https://github.com/thesofproject/sof-bin
- Download latest release and install it:

`cd <sof-bin-archive>`

`./install.sh <version>` eg. `./install.sh v1.9`

- Reboot 
- Check that audio works

## Still Broken
- Fingerprint sensor still doesn't works cause no drivers for it (https://gitlab.freedesktop.org/libfprint/libfprint/-/issues/112)
- Poor audio quality because only 2 of 4 dynamics are works (here is the fix for 2020 model but still not works for my 2021 lineup, https://github.com/samuelmatn/guides/blob/main/manjaro-matebook.md#set-up-40-surround-speakers)
