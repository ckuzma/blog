---
layout: post
title: Manipulate My House Via Twitter
date: '2015-01-14T17:03:00.000-08:00'
author: Christopher Kuzma
tags:
- wit
- hack
- cloud
- arduino
- esp8266
- wifi
- java
- nlp
modified_time: '2015-01-14T17:03:06.979-08:00'
thumbnail: http://2.bp.blogspot.com/-84QPVIoThMY/VLcO4lErdHI/AAAAAAAAGc8/5I5Ba04uw5s/s72-c/DSC_7370.jpg
---

<table align="center" cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="http://2.bp.blogspot.com/-84QPVIoThMY/VLcO4lErdHI/AAAAAAAAGc8/5I5Ba04uw5s/s1600/DSC_7370.jpg" imageanchor="1" style="margin-left: auto; margin-right: auto;"><img border="0" src="http://2.bp.blogspot.com/-84QPVIoThMY/VLcO4lErdHI/AAAAAAAAGc8/5I5Ba04uw5s/s1600/DSC_7370.jpg" height="263" width="400" /></a></td></tr><tr><td class="tr-caption" style="text-align: center;">The actual setup as it stands.</td></tr></tbody></table>First <a href="http://blog.christopherkuzma.com/2014/10/wittylights.html" target="_blank">I combined an Arduino with an API</a> that processes commands written in natural language. Then I gave the same Arduino <a href="http://blog.christopherkuzma.com/2015/01/arduino-controlled-christmas-lights.html" target="_blank">the ability to control high-voltage</a> circuits. Next I threw <a href="http://blog.christopherkuzma.com/2015/01/building-web-controlled-wifi-enabled.html" target="_blank">a WiFi module into the mix</a> to for easy wireless control. And now I've come full circle and put it all together. You can now control real, physical lights in my house by tweeting commands to <a href="https://twitter.com/WittyDevices" target="_blank">@WittyDevices</a>. At the moment it's only controlling four small red-colored LEDs, but it could just as easily be wired up to anything using the 110v power control box I built.<br /><br /><table align="center" cellpadding="0" cellspacing="0" class="tr-caption-container" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="http://1.bp.blogspot.com/-jXdIFbVxOpY/VLcRTXaGQ6I/AAAAAAAAGdI/yuj4wcZdRrk/s1600/Screen%2BShot%2B2015-01-14%2Bat%2B7.51.23%2BPM.png" imageanchor="1" style="margin-left: auto; margin-right: auto;"><img border="0" src="http://1.bp.blogspot.com/-jXdIFbVxOpY/VLcRTXaGQ6I/AAAAAAAAGdI/yuj4wcZdRrk/s1600/Screen%2BShot%2B2015-01-14%2Bat%2B7.51.23%2BPM.png" height="262" width="400" /></a></td></tr><tr><td class="tr-caption" style="text-align: center;">The tweets which led to the illumination scheme in the above picture.</td></tr></tbody></table>The Java application powering the whole thing is running in the cloud and should thus be accessible 24/7 (unless you see a tweet indicating otherwise from @WittyDevices). The physical board might lose its connectivity now and then, but it will instantly resume its program once it is back online. Details to follow... I have a few small updates to make to the original project's source code.