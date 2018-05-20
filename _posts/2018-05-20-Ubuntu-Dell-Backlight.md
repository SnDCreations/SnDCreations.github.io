---
title: "Keyboard Backlight - Dell - Ubuntu"
layout: post
date: 2018-05-20
---



I have realised my Dell laptop keyborad backlight doesn't light up in Ubuntu. So did some browsing and changed the config file.

1. Set the brightness level to > 0 using below, you need to change the value using super user (or root). Open the config using nano editor.

```
sudo nano /sys/devices/platform/dell-laptop/leds/dell\:\:kbd_backlight/brightness

```
change the value 0, I have changed it to 2, then save the config.

2. Also if required we can set the timeout of the keyboard backlight.

```
sudo nano /sys/devices/platform/dell-laptop/leds/dell\:\:kbd_backlight/stop_timeout

```
***

More information can be found in [askubuntu](https://askubuntu.com/questions/763552/keyboard-backlight-keeps-going-on-in-ubuntu-16-04-lts)

