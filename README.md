# cachyos-xfce-settings

CachyOS xfce4 settings

**XFCE** is a simple desktop environment emphasizes on stability and lightweightness. However, XFCE's default looks like it's from 2000s era. This setting aims to make XFCE looks polished and modern on first glance while still retain the spirit of XFCE.

This repository contains configuration files for various programs and tools used in the CachyOS XFCE operating system. Feel free to customize your system from these configurations!

Thank you for using CachyOS XFCE Settings. We hope you enjoy desktop that stays for years without a surprise!

## Themes
default xfce themes, icons, and cursor are still shipped by they won't be presented as default
- gtk theme and xfwm/xfwl theme: **whitesur dark gtk** - whitesur light is also available
- icon theme: **papirus-dark** - papirus-light and papirus are also available
- cursor: **bibata-modern-ice** - bibata-modern-classic is also available

## Additional changes
Some minor changes are applied to improve QoL by default

## Limit
lightdm stays untouched because that thing can be fragile but users are free to config it easily with`lightdm-gtk-greeter-setting` GUI

## To-Do-List
- testing on real hardware for possible edge cases
- waiting for xfwl integration on upstream arch

## Dependencies
### XFCE Packages
- exo
- garcon
- xfce4-appfinder
- xfce4-panel
- xfce4-power-manager
- xfce4-session
- xfce4-settings
- xfce4-terminal
- xfconf
- xfdesktop
- xfwm4
- **xfwl4 (soon!)**
### Thunar Stuff
- thunar
- thunar-volman
- tumbler
- thunar-archive-plugin
- thunar-media-tags-plugin
- gvfs
### XFCE Plugins
- xfce4-whiskermenu-plugin
- xfce4-docklike-plugin
- xfce4-pulseaudio-plugin
- xfce4-xkb-plugin
### Default XFCE Apps
- xfce4-screenshooter
- xfce4-screensaver
- xfce4-taskmanager
- ristretto
- parole
- mousepad
- mugshot
### Other apps that belong here
- mate-calc
- engrampa
- font-manager
- lightdm-gtk-greeter-settings
- network-manager-applet
- blueman
## Backends
- gnome-keyring
- bluez
- bluez-utils
### Only font that would be shipped here
- noto-fonts             
### Basic ricing stuff
- cachyos-wallpapers
- papirus-icon-theme
### Display Manager
- lightdm
- lightdm-gtk-greeter
### You need this to run X11 apps on XFWL
- xorg-xwayland
