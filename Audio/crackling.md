---
title: Weird Clicking Sound in the Background
description: 
published: true
date: 2024-03-05T00:42:48.927Z
tags: 
editor: markdown
dateCreated: 2024-03-05T00:40:16.704Z
---


Run the following commands: 
`echo "0" | sudo tee /sys/module/snd_hda_intel/parameters/power_save`

`echo "options snd_hda_intel power_save=0" | sudo tee -a /etc/modprobe.d/audio_disable_powersave.conf`

[Credit](https://askubuntu.com/questions/1230833/annoying-click-popping-sound-on-ubuntu-20-04/1230834#1230834)
