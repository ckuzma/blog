Version 2.0

A little over a year ago I built an Arduino-controlled electrical box connected to the web via an ESP8266 WiFi board. With an Arduino Uno rattling around loose in there, it was anything but pretty to look at and undoubtedly a fire hazard. The whole setup also felt unnecessarily large, a feeling that may or may not have been prompted by the sudden flood of commercially produced IoT-esque power switches flooding the market at around the same time. So, many months ago, I set out to give my solution a facelift.

The physical dimensions of the Uno and the 4-channel relay switch employed in the project did not lend themselves easily to being crammed into a smaller space. Eventually I saw no alternative but to swap out the Uno for a Nano and hope that the board would supply enough power to run everything reliably. I then grabbed a saw and went to town on the electrical box.

Everything is hidden just behind the power plugs.

It turned out to be a perfect fit, with a bit of room to spare. With each component either glued into position or secured with mounting screws, the end result is an equally capable solution in roughly half the size of the original. I even found space on which to proudly write the project version number.

The only thing not properly handled- apart from a real box cover to prevent someone from sticking their fingers in when the power lines are live- is getting input power to the Arduino Nano itself. It still requires USB power routed through a hole in the side of the box. Not an elegant solution, but it does work.

Hopefully, once my heater project is finished, I'll find a way to get this added into the same system for more complete DIY home automation.