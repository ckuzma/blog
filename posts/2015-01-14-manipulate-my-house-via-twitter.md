The actual setup as it stands.

First I combined an Arduino with an API that processes commands written in natural language. Then I gave the same Arduino the ability to control high-voltage circuits. Next I threw a WiFi module into the mix to for easy wireless control. And now I've come full circle and put it all together. You can now control real, physical lights in my house by tweeting commands to @WittyDevices. At the moment it's only controlling four small red-colored LEDs, but it could just as easily be wired up to anything using the 110v power control box I built.

The tweets which led to the illumination scheme in the above picture.

The Java application powering the whole thing is running in the cloud and should thus be accessible 24/7 (unless you see a tweet indicating otherwise from @WittyDevices). The physical board might lose its connectivity now and then, but it will instantly resume its program once it is back online. Details to follow... I have a few small updates to make to the original project's source code.