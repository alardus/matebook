# How to cook Linux Mint 20.3 on MateBook X Pro 2021 

## Final Overview
<pre><b>             ...-:::::-...</b>                 <font color="#8AE234"><b>alardus</b></font>@<font color="#8AE234"><b>matebook</b></font> 
<b>          .-MMMMMMMMMMMMMMM-.</b>              ---------------- 
<b>      .-MMMM</b><font color="#8AE234"><b>`..-:::::::-..`</b></font><b>MMMM-.</b>          <font color="#8AE234"><b>OS</b></font>: Linux Mint 20.3 x86_64 
<b>    .:MMMM</b><font color="#8AE234"><b>.:MMMMMMMMMMMMMMM:.</b></font><b>MMMM:.</b>        <font color="#8AE234"><b>Host</b></font>: MACHD-WXX9 M1090 
<b>   -MMM</b><font color="#8AE234"><b>-M---MMMMMMMMMMMMMMMMMMM.</b></font><b>MMM-</b>       <font color="#8AE234"><b>Kernel</b></font>: 5.14.0-1020-oem 
<b> `:MMM</b><font color="#8AE234"><b>:MM`  :MMMM:....::-...-MMMM:</b></font><b>MMM:`</b>    <font color="#8AE234"><b>Uptime</b></font>: 5 hours, 27 mins 
<b> :MMM</b><font color="#8AE234"><b>:MMM`  :MM:`  ``    ``  `:MMM:</b></font><b>MMM:</b>    <font color="#8AE234"><b>Packages</b></font>: 2091 (dpkg), 15 (flatpak) 
<b>.MMM</b><font color="#8AE234"><b>.MMMM`  :MM.  -MM.  .MM-  `MMMM.</b></font><b>MMM.</b>   <font color="#8AE234"><b>Shell</b></font>: bash 5.0.17 
<b>:MMM</b><font color="#8AE234"><b>:MMMM`  :MM.  -MM-  .MM:  `MMMM-</b></font><b>MMM:</b>   <font color="#8AE234"><b>Resolution</b></font>: 3000x2000 
<b>:MMM</b><font color="#8AE234"><b>:MMMM`  :MM.  -MM-  .MM:  `MMMM:</b></font><b>MMM:</b>   <font color="#8AE234"><b>DE</b></font>: Cinnamon 
<b>:MMM</b><font color="#8AE234"><b>:MMMM`  :MM.  -MM-  .MM:  `MMMM-</b></font><b>MMM:</b>   <font color="#8AE234"><b>WM</b></font>: Mutter (Muffin) 
<b>.MMM</b><font color="#8AE234"><b>.MMMM`  :MM:--:MM:--:MM:  `MMMM.</b></font><b>MMM.</b>   <font color="#8AE234"><b>WM Theme</b></font>: Mint-Y-Dark-Aqua (Mint-Y) 
<b> :MMM</b><font color="#8AE234"><b>:MMM-  `-MMMMMMMMMMMM-`  -MMM-</b></font><b>MMM:</b>    <font color="#8AE234"><b>Theme</b></font>: Mint-Y-Aqua [GTK2/3] 
<b>  :MMM</b><font color="#8AE234"><b>:MMM:`                `:MMM:</b></font><b>MMM:</b>     <font color="#8AE234"><b>Icons</b></font>: Mint-Y-Aqua [GTK2/3] 
<b>   .MMM</b><font color="#8AE234"><b>.MMMM:--------------:MMMM.</b></font><b>MMM.</b>      <font color="#8AE234"><b>Terminal</b></font>: gnome-terminal 
<b>     &apos;-MMMM</b><font color="#8AE234"><b>.-MMMMMMMMMMMMMMM-.</b></font><b>MMMM-&apos;</b>       <font color="#8AE234"><b>CPU</b></font>: 11th Gen Intel i7-1165G7 (8) @ 4.700GHz 
<b>       &apos;.-MMMM</b><font color="#8AE234"><b>``--:::::--``</b></font><b>MMMM-.&apos;</b>         <font color="#8AE234"><b>GPU</b></font>: Intel Device 9a49 
<b>            &apos;-MMMMMMMMMMMMM-&apos;</b>              <font color="#8AE234"><b>Memory</b></font>: 2793MiB / 15806MiB 
<b>               ``-:::::-``</b>
                                           <span style="background-color:#2E3436"><font color="#2E3436">   </font></span><span style="background-color:#CC0000"><font color="#CC0000">   </font></span><span style="background-color:#4E9A06"><font color="#4E9A06">   </font></span><span style="background-color:#C4A000"><font color="#C4A000">   </font></span><span style="background-color:#3465A4"><font color="#3465A4">   </font></span><span style="background-color:#75507B"><font color="#75507B">   </font></span><span style="background-color:#06989A"><font color="#06989A">   </font></span><span style="background-color:#D3D7CF"><font color="#D3D7CF">   </font></span>
                                           <span style="background-color:#555753"><font color="#555753">   </font></span><span style="background-color:#EF2929"><font color="#EF2929">   </font></span><span style="background-color:#8AE234"><font color="#8AE234">   </font></span><span style="background-color:#FCE94F"><font color="#FCE94F">   </font></span><span style="background-color:#729FCF"><font color="#729FCF">   </font></span><span style="background-color:#AD7FA8"><font color="#AD7FA8">   </font></span><span style="background-color:#34E2E2"><font color="#34E2E2">   </font></span><span style="background-color:#EEEEEC"><font color="#EEEEEC">   </font></span>
</pre>

<pre>
    <font color="#729FCF"><b>Graphics:  Device-1:</b></font> Intel <font color="#729FCF"><b>driver:</b></font> i915 <font color="#729FCF"><b>v:</b></font> kernel 
           <font color="#729FCF"><b>Display:</b></font> x11 <font color="#729FCF"><b>server:</b></font> X.Org 1.20.13 <font color="#729FCF"><b>driver:</b></font> modesetting <font color="#729FCF"><b>unloaded:</b></font> fbdev,vesa <font color="#729FCF"><b>resolution:</b></font> 3000x2000~60Hz 
           <font color="#729FCF"><b>OpenGL:</b></font> <font color="#729FCF"><b>renderer:</b></font> Mesa Intel Xe Graphics (TGL GT2) <font color="#729FCF"><b>v:</b></font> 4.6 Mesa 21.0.3 
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
- Wi-Fi
- Hibernation

## What's Bad (out of the box)
- Touchpad and gestures
- Tochscreen
- FN keys
- Bluetooth
- Camera
- Mic
- Poor audio quality because only 2 of 4 dynamics are works (here is the fix for 2020 model but still not works for my 2021 lineup, https://github.com/samuelmatn/guides/blob/main/manjaro-matebook.md#set-up-40-surround-speakers)
- Fingerprint sensor doesn't works (Goodix GXFP5187 still has no drivers, https://gitlab.freedesktop.org/libfprint/libfprint/-/issues/112)

## Installation
### Disabling Secure Boot
- Press F2 on boot stage
- Disable "Secure boot"
- Save and Exit

### Booting to Installer
- Press F12 on boot stage
- Select USB flash with Mint

### Installing Mint
- Select "Boot"

## Fixes

### Fix many issues with one tap
We need to switch to the latest Ubuntu OEM kernel (like 5.14 or above) with our hardware support:

`sudo apt install linux-oem-20.04d`
`sudo apt remove linux-generic linux-headers-generic linux-image-generic`

- Reboot
- When GRUB shows, select "Advanced Params"
- Select lastest kernel version and boot into it

## Still Broken
- Bluetooth
- Fingerprint sensor still doesn't works cause no drivers for it (https://gitlab.freedesktop.org/libfprint/libfprint/-/issues/112)
- Poor audio quality because only 2 of 4 dynamics are works (here is the fix for 2020 model but still not works for my 2021 lineup, https://github.com/samuelmatn/guides/blob/main/manjaro-matebook.md#set-up-40-surround-speakers)
