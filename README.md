# !!! !!! IN PROGRESS !!! !!!

# void-audiobox
Publish Voidlinux XBPS repo (multi-arch) for squeezelite AudioBox player

This repo support the ARCH x86_64 and ARM aarch64 / armv7l / armv6l

Thanks to all the cracks from LYRION COMMUNITY https://forums.lyrion.org

and ralph-irving for the code https://github.com/ralph-irving/squeezelite

# INSTALL the OS

This repository is for void-linux-musl linux

Please download for your ARCH:

### x86_64 live iso
https://repo-default.voidlinux.org/live/current/void-live-x86_64-musl-20250202-base.iso

### rpi-aarch64 platform image
https://repo-default.voidlinux.org/live/current/void-rpi-aarch64-musl-20250202.img.xz

### rpi-armv7l platform image
https://repo-default.voidlinux.org/live/current/void-rpi-armv7l-musl-20250202.img.xz

### rpi-armv6l platform image
https://repo-default.voidlinux.org/live/current/void-rpi-armv6l-musl-20250202.img.xz

# FIRST INIT
Check the IP of your device in our router

Login with SSH ' ssh root@<IP_off_your_device> ' or direct at your terminal.

Default User is ' root ' with default password ' voidlinux '

First change the password with ' passwd '

Update the void OS

' xbps-install -Suy xbps '

Import this repo
 
' echo "repository=https://void-audiobox.github.io/xbps/aarch64-musl" | sudo tee /etc/xbps.d/void-audiobox.conf '

' xbps-install -Suy '

Please type ' Y ' to import the Fingerprint: 04:5b:56:1d:be:6a:69:f7:d6:a2:cf:2f:52:b3:25:79

## Install the squeezelite package

' xbps-install -S squeezelite '

Search for output devive

' squeezelite -l'

Example for Pi500

Output devices:

  - null                           - Discard all samples (playback) or generate zero samples (capture)

  - default                        - Default Audio Device

  - sysdefault                     - Default Audio Device

  - default:CARD=vc4hdmi0          - vc4-hdmi-0, MAI PCM i2s-hifi-0 - Default Audio Device

  - sysdefault:CARD=vc4hdmi0       - vc4-hdmi-0, MAI PCM i2s-hifi-0 - Default Audio Device

  - hdmi:CARD=vc4hdmi0,DEV=0       - vc4-hdmi-0, MAI PCM i2s-hifi-0 - HDMI Audio Output

  - default:CARD=vc4hdmi1          - vc4-hdmi-1, MAI PCM i2s-hifi-0 - Default Audio Device

  - sysdefault:CARD=vc4hdmi1       - vc4-hdmi-1, MAI PCM i2s-hifi-0 - Default Audio Device

  - hdmi:CARD=vc4hdmi1,DEV=0       - vc4-hdmi-1, MAI PCM i2s-hifi-0 - HDMI Audio Output

Start your squeezelite in the terminal and look at your LMS (Lyrion Media Server) to control the player

' squeezelite -o "hdmi:CARD=vc4hdmi0,DEV=0" -s <LMServer>[:<port>] '

