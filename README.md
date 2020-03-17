### [Blog Homepage](https://github.com/ckuzma/blog) | [About the Author](https://ckuzma.github.io/) | [Posts Archive](/posts)
# The Blog of Christopher Kuzma

#### 16.03.2020
### NXP HoverGames Drone Build

> Original Project / Contest Submission on Hackster: https://www.hackster.io/kuzma/abandoned-bonfire-detector-91ef7d

The elevator pitch for this contest submission? _"Keep beachgoers safe by identifying still-hot bonfires, even when they've been put put out and covered."_  While the drone still has yet to achieve flight thus cannot even begin to come close to fulfilling that promise, I thought the build process for the drone was interesting enough to warrant sharing nonetheless.

The original purpose of the project was to build a drone that could identify hidden hotspots on the ground (read: improperly extinguished campfires) and report them to a human operator.  Were I to have had some success in achieving this, I would have submitted my drone schematics and code to Hackster.io as part of the [HoverGames Challenge 1: Fight Fire with Flyers](https://www.hackster.io/contests/hovergames#category-547) contest sponsored by NXP.

---

**Project Timeline:**
- 6/4/2019: Project idea submitted
- 7/11/2019: Telemetry kit and HoverGames drone kit ordered
- 7/19/2019: Telemetry kit received
- 7/22/2019: HoverGames drone kit received, PX4 Firmware repository forked
- 8/2/2019: Began assembling drone kit
- 8/4/2019: Finished assembling drone pending final motor wiring and FMU setup
- 8/6/2019: Camera gimbal ordered from AliExpress
- 8/13/2019: Registered drone as sUAS with the FAA, wrote PX4 firmware to FMU and started calibration
- 8/19/2019: Camera gimbal delivered
- 9/3/2019: Stabilized camera gimbal installed, telemetry firmware updated, ESCs calibrated
- 9/9/2019: Removed throttle return spring from TX, affixed FAA registration to the drone in preparation for first flight
- 9/10/2019: First experimentation session with Pixy2 camera
- 11/?/2019: Realized the (il)legality of flying in the area and maiden flight postponed indefinitely
- 12/26/2019: Sent email stating inability to follow-through with the competition and put all of my work for the contest on hold indefinitely
- 1/8/2020: Told by Hackster team to submit project as-is
- 1/26/2020: Submitted contest entry incomplete with the hope that the assembly photos might be useful to someone in the future

**Drone Assembly**

![drone15](posts/2020/media/hovergames_drone/drone/15.jpeg)

<details><summary>Click to view additional photos</summary>

- ![drone01](posts/2020/media/hovergames_drone/drone/01.jpeg)
- ![drone02](posts/2020/media/hovergames_drone/drone/02.jpeg)
- ![drone03](posts/2020/media/hovergames_drone/drone/03.jpeg)
- ![drone04](posts/2020/media/hovergames_drone/drone/04.jpeg)
- ![drone05](posts/2020/media/hovergames_drone/drone/05.jpeg)
- ![drone06](posts/2020/media/hovergames_drone/drone/06.jpeg)
- ![drone07](posts/2020/media/hovergames_drone/drone/07.jpeg)
- ![drone08](posts/2020/media/hovergames_drone/drone/08.jpeg)
- ![drone09](posts/2020/media/hovergames_drone/drone/09.jpeg)
- ![drone10](posts/2020/media/hovergames_drone/drone/10.jpeg)
- ![drone11](posts/2020/media/hovergames_drone/drone/11.jpeg)
- ![drone12](posts/2020/media/hovergames_drone/drone/12.jpeg)
- ![drone13](posts/2020/media/hovergames_drone/drone/13.jpeg)
- ![drone14](posts/2020/media/hovergames_drone/drone/14.jpeg)
</details>

**Transmitter Mod (Throttle Spring Removal)**

![controller02](posts/2020/media/hovergames_drone/controller/002.jpg)

<details><summary>Click to view additional photos</summary>

- ![controller01](posts/2020/media/hovergames_drone/controller/001.jpg)
- ![controller03](posts/2020/media/hovergames_drone/controller/003.jpg)
- ![controller04](posts/2020/media/hovergames_drone/controller/004.jpg)
</details>

Most transmitters designed for aerial R/C vehicles lack a throttle-stick return spring in order to facilitate the holding of a given throttle input value.  Transmitters with this spring actively attempt to return the throttle input to 50% without a counteracting force provided by the operator's fingers.  This makes certain aspects of flying (hovering, landing, maintaining speed) difficult for helicopters, quadcopters, and airplanes alike.

The FlySky FS-i6S provided with the drone kit is something of a multipurpose transmitter and thus has this return spring installed at the factory.  I decided to remove it as I have with other transmitters (which seems to be the same decision taken by the NXP team given the photo of their transmitter in the Gitbook documentation), which was a relatively straightforward process.  Simply remove the four screws hidden underneath the rubber transmitter grips, carefully open up the transmitter case, identify the return spring assembly for the throttle stick (one spring plus two small plastic lever components), and set them aside for future re-installation if so desired.

**Pixy2 Camera Experiments**

![pixy](posts/2020/media/hovergames_drone/pixy/001.jpg)

_[Note: I never actually completed any actual experiments with the Pixy2 camera, hence why this section is blank.]_

#### 10.03.2020
### Turntable Mod: Replacing LED on Teac TN-300SE

![the problem](posts/2020/media/turntable_mod/IMG_3214.jpg)

See that bright blue, glaring LED indicator light on the record player above?  That tiny little thing has been driving me up the wall for months now.  The problem with it occurs at night: when I attempt to listen to some records when living room is dimly lit, accurately dropping the tonearm on the lead-in groove of a record is nearly impossible thanks to the blinding glare of the power status light.

After months of attempting to block out the light with my thumb while I'm cueing up a new disk (or giving up and employing a flashlight to counteract the glare), I decided to take matters into my own hands and address the issue.  Expecting to find a SMD-type LED soldered to a control board, I cracked open my Teac TN-300SE with the intention of somehow diffusing the light output of the diode itself.

![bottom panel removed](posts/2020/media/turntable_mod/IMG_3215.jpg)

With the bottom panel removed, I am glad to see that the part I'm interested in is indeed an independent control board.  (Read: if I were to break it, I wouldn't have to replace the entire record player.)

![control board bottom](posts/2020/media/turntable_mod/IMG_3216.jpg)

The bottom of the control board hinted that it might be possible for me to bypass the LED by shorting its two connection terminals with some solder.  The plan at this point was still to scribble a bit of Sharpie or scratch up the diode a bit and see if that accomplished enough of a dimming effect.

![control board top](posts/2020/media/turntable_mod/IMG_3222.jpg)

Turned over, the LED makes itself immediately obvious compared to the two spring-loaded pot switches.  Realizing that I might actually be able to (messily) remove the diode entirely and replace it with a much less annoying red one, despite not having access to a solder remover, I plugged in my soldering iron and fished out some solder.

![replaced diode](posts/2020/media/turntable_mod/IMG_3224.jpg)

Somehow, despite almost completely ruining a solder pad on the circuit board, I managed to successfully replace the blue diode with a red LED.  At this point I put everything back together again, testing everything intermittently as I did so.

![back together demo](posts/2020/media/turntable_mod/IMG_3226.jpg)

And there's the finished result!  Though not immediately obvious in this well-lit photograph, the glare emitted by the red LED is virtually non-existent compared to its predecessor.  The end result is a much more pleasant experience of playing and changing records at night in a room illuminated by candles or dim lights.  I'd call that a success.

### [View older posts...](/posts)