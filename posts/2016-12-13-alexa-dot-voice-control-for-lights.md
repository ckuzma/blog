# Alexa Dot Voice Control for Lights

The past few weeks have seen me hacking together a number of small projects from [Conway's Game of Life on an OLED](https://github.com/ckuzma/nodemcu_oled_sketches/blob/master/nodemcu_oled_conway.ino) screen to an [informational bot giving real-time radar information for Amazon Alexa](https://github.com/ckuzma/atc_alexa). Today I'm sharing a project I recently put some finishing touches on: Alexa voice-control for lights using nothing more than a NodeMCU. The firmware code is based largely off of someone else's project aimed at getting an Arduino board to do the exact same thing, but I made a few key modifications:
- Major refactor because the original code was both messy and slow (sorry it's true!)
- The GPIO pin is set to voltage up by default (for offline use without WiFi / Alexa)
- Implemented a WiFi Manager, negating the use for hard-coded WiFi credentials

The finished prototype was connected to a single LED, as you can see in the demo video here:
- https://www.youtube.com/watch?v=yYnQ7DLzWcU

I wasn't entirely sure how I wanted to make a more permanent implementation, but then I noticed I had not one, not two, but five NodeMCUs sitting around in a bin. It thus didn't take long before I'd committed one of them permanently to this project. I also decided to hardwire the end result directly to the end of some string-light LEDs.

[Similar](http://blog.christopherkuzma.com/2015/02/4x4x4-led-cube-powered-by-arduino.html) to some of my [prior](http://blog.christopherkuzma.com/2016/03/4x4x4-led-cube-take-two.html) [projects](http://blog.christopherkuzma.com/2016/09/weather-widget-nodemcu-amoled.html), I sandwiched the solder connections and wiring between two prototyping boards. This enabled me to wind the cord running to the LED lights around the pins and thus hopefully alleviate stress and prevent the connections from breaking loose.

While I'm not entirely happy with the result- mostly because it would be far too easy for something to short pins on the NodeMCU- it's at the point where any additional work put into it will only result in minimal improvements.  And what would project documentation be without a link to the code repo? You can find it here:
- https://github.com/ckuzma/nodemcu-as-arduino/tree/master/Sketches/Alexa/AlexaWemoSwitch