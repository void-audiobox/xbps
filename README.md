# void-audiobox
Publish Voidlinux XBPS repo (multi-arch) for squeezelite AudioBox player

Thanks to all the cracks from LYRION COMMUNITY https://forums.lyrion.org

and ralph-irving for the code https://github.com/ralph-irving/squeezelite

# INSTALL the OS

This repository is for void-linux-musl linux

Please download for your ARCH:

### x86_64 live iso
https://repo-default.voidlinux.org/live/current/void-live-x86_64-20250202-base.iso



echo "repository=https://void-audiobox.github.io/xbps/aarch64-musl" | sudo tee /etc/xbps.d/void-audiobox.conf

## Update the repo

sudo xbps-install -S [press "yes"]


