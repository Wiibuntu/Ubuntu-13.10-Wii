# Ubuntu Server 13 Nintendo Wii



This repository contains images of Ubuntu Server 13 for the Wii. Downloads are found to your right (on desktop).

# About The Project
Trying to bring newer versions of Ubuntu to the Wii has been a project of mine for a while. Many trial and errors.
This versions actually build somewhat off of [Wii-Linux-NGX](https://github.com/neagix/wii-linux-ngx)
But this version uses the same bootloader with a different kernel, a newer one. And it also boots Ubuntu 13 instead of Debian 8.

You have 2 Kernels to choose from via Gumboot. More info in "How To Boot".

# How to Install (Homebrew Needed!)
In the download section you will find a .img file. That file will contain two partitions: a fat32 partition and a ext4 partition. The fat32 partition will contain the Linux loader for the Homebrew Channel.

Just flash this image to an SD Card (2GB or more needed!)

*TO RUN OVER USB, YOU MUST RECOMPILE THE KERNEL!*
https://github.com/neagix/wii-linux-ngx#building-the-kernel 

Kernels Used [STABLE](https://github.com/Wii-Linux/wii-linux-ngx/tree/stable-v3.x) [UNSTABLE](https://github.com/Wii-Linux/wii-linux-ngx/tree/stable-v3.14.19)

(Baedit has not been tested for either of these kernels)

# How To Boot
You will load up the homebrew channel to see its empty, thats normal. Simply press the home button and click "Launch BootMii"
That will instead load a bootloader known as Gumboot. More on Gumboot [here](https://neagix.github.io/gumboot/).
In order to select a different item in gumboot you MUST have a gamecube controller plugged in. But, thankfully it will auto boot in 30 seconds.

By Default gumboot will load the the Stable kernel. If you have a gamecube controller you can choose the other option below the default top option, which is a newer kernel but is also quite broken as you will see if you boot from it.

![alt text](https://github.com/Wiibuntu/Ubuntu14-Wii/blob/main/Screenshots/Screen%20Shot%202023-10-17%20at%205.50.29%20PM.png)

![alt text](https://github.com/Wiibuntu/Ubuntu-13.10-Wii/blob/main/Screenshots/Screenshot%202024-03-11%20115913.png?raw=true)

You will see an errors have been found at / dialog, im no pro, so I did most likely mess something up, but press I on a keyboard to ignore this and continue to boot.

![alt text](https://github.com/Wiibuntu/Ubuntu-13.10-Wii/blob/main/Screenshots/Screenshot%202024-03-11%20115949.png?raw=true)

# Login

user- ubuntu

pass- ubuntu

![alt text](https://github.com/Wiibuntu/Ubuntu-13.10-Wii/blob/main/Screenshots/Screenshot%202024-03-11%20120047.png?raw=true)

# WiFI Config
Its as simple as using the "whiite-ez-wifi-config" file located in "/home/ubuntu" and setting up for wifi!

If that doesnt work please use the command "sudo nano /etc/network/interfaces" and add the ssid and passkey yourself.

![alt text](https://github.com/Wiibuntu/Ubuntu-13.10-Wii/blob/main/Screenshots/Screenshot%202024.png?raw=true)

# Swapfile
Swapfile has already been setup but is small and can be made bigger if you wish.

Swapfile is needed to even run basic tasks but was kept small in order to keep download size as small as possible. 

![alt text](https://github.com/Wiibuntu/Ubuntu-13.10-Wii/blob/main/Screenshots/Screenshot%202024-03-11%20120110.png?raw=true)

# Contact
Contact me at wiibuntuhelp@gmail.com I will always try to help if I can and have the time to do so.
