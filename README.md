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


echo "repository=https://void-audiobox.github.io/xbps/aarch64-musl" | sudo tee /etc/xbps.d/void-audiobox.conf

## Update the repo

sudo xbps-install -S [press "yes"]


