#### 16.02.2021
### Adventures in 3D Printing: Nixie Clock Stands

![Finished stands on working clock.](media/nixie_stand/000.jpeg)

> The completed stand running my own [slightly modified version](https://github.com/ckuzma/NixieTubesShieldNCS314) of the [official stock firmware](https://github.com/afch/NixeTubesShieldNCS314).  (Most notably the blinking neon digit indicators have been disabled.)

Despite investing a not-insignificant amount of time and energy into [the woden case I built for my nixie tube clock last year](../2020/2020-04-18-nixie-tube-box-case-part-2.md), I could never shake the feeling that it was just temporary.  Be it the lack of access to the control buttons, the horrendously abrasive sound that would be emitted by the lone tilt screw when dragged across a surface, or the somewhat poor appearance of the wood finish itself, I just never loved it.

My search for an upgrade inevitably brought me to Thingiverse, where a [simply designed stand](https://www.thingiverse.com/thing:2232491) by [TimeWaster](https://www.thingiverse.com/TimeWaster) caught my eye.  Unfortunately, I was so excited by my finding that I only noticed that it was designed around a GRA & AFCH-made nixie board, but not _which_ board it was specifically designed for.  As a result of this I learned the hard way that the NCT412 doesn't share enough similar physical features with my NCS312 to be compatible.

Not to be dissuaded, I opted to continue the spirit of hard learning and teach myself how to use FreeCAD for creating parts of a more technical manner than allowed by TinkerCAD.  Having read numerous articles extolling the virtues of FreeCAD for more advanced hobbyists I was ingrigued by this lauded, multi-platform, and GPL2+ licensed CAD software.  At the very least it seemed like the right next step to take towards developing 3D-printed parts of my own.

Admittedly, things were off to a rough start.  My first attempt at measuring (using an imperial-marked ruler) the spaces between the cornermost mounting holes, converting the units, plotting them out in space in FreeCAD, and then creating 2mm-thick rectangles with holes cut out of them to check for proper fit was unsuccessful.  I realized that replicating the [success of my last project](2021-02-16-luci-housing.md) would be a lot harder than I'd imagined, and I immediately began scouring the internet for some help.

That's when I stumbled across [a 3D model of the NCS312 board, created by GRA & AFCH themselves, hosted freely on their own website](https://gra-afch.com/downloads/drawings/shield-board-ncs312-shield-for-nixie-clocks-3).  With this handy resource loaded into FreeCAD, I was able to make the screw holes in the stand I'd designed line up perfectly with those in the NCS312 unit, and made some additional tweaks to the angle at which the complete nixie clock would be held.

![3D stand rendering.](media/nixie_stand/3d-stands.png)

> Curiously enough, the holes in the right-side stand are offset to the left, causing the right stand to protrude a bit farther than the actual right-side edge of the clock.  If this bothers me enough I'll fix that in the future.

![Real stands seen at an angle.](media/nixie_stand/001.jpeg)
![Stands seen from behind.](media/nixie_stand/002.jpeg)
![Detail on printed standoff spacers.](media/nixie_stand/003.jpeg)

- https://github.com/ckuzma/nixie-clock-stands