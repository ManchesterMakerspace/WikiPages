---
title: MX Linux Customization
description: 
published: true
date: 2022-05-03T16:06:11.531Z
tags: 
editor: undefined
dateCreated: 2022-05-03T16:02:49.334Z
---

# Standard Linux Install

## Install Media
We are using MX21.1_x64 with the XFCE desktop https://mxlinux.org/download-links/ 
Computer names are `mm-linux-#` and are on the `manchestermakerspace.org` domain.
User is `makerspace`
Enable autologin
Enable 24-hour time

## Apps
Install these packages from the standard repos
```
sudo apt install inkscape openscad solaar gimp flameshot krita audacity
```

## Wallpaper
Use the vectorized surge mural, zoomed (not stretched)

## Thunar (file explorer)
In preferences, change the open behavior to double click, not single click.

## Taskbar
Make it a horizontal deskbar with the app menu on the far left (start) not end.

## Cura
Cura is available as an AppImage (ew, gross, yes, but...). Details to come.

## Sublime Text
via https://www.sublimetext.com/docs/linux_repositories.html 

```
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
sudo apt-get install apt-transport-https
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update
sudo apt-get install sublime-text
```


## Hardware Thad Likes
Keyboard: Lenovo Preferred Pro
Mouse: Logitech M510