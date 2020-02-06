YouTube is rife with videos of houses adorned with Christmas lights made into into spectacular- if over the top- light shows. These are typically synchronized to music and generally serve to make ordinary holiday decorations look, well, kind of boring. I used to watch these videos and wonder at the amount of time that was spent building and installing them. Surely such a project was one I'd never bother with.

That is until I realized I had most of the parts necessary to build such a thing right under my own nose. This year I decided to find out just how hard it really is to build a custom light show. I disassembled my @WittyDevices project, picked up a couple of new parts, and got to work.

Parts used:
- 1 x 4-socket Electrical Box
- 2 x 2-plug Sockets
- 1 x 4-channel Relay Switch Board
- 1 x Arduino Uno R3 Kit w/Wires
- Spare wiring, solder, time, etc.
- 4-channel relay wired up and glued into the electrical box

The most important part of this project is the relay board. Arduino controllers aren't built to handle the 120v output of a standard wall plug. This is the first and most obvious obstacle that needs to be overcome in this project. Relays are a great way to handle the problem, taking lower voltage commands from a control circuit and applying them to isolated circuits operating at much greater voltages. For simplicity's sake (and my own safety), I decided to purchase a prebuilt board instead of attempting to build one myself.

Sockets with plug numbers marked.

In the interest of safety I also decided that it would be better to encapsulate everything within an electrical box. I also decided against splicing perfectly good wire leads off of light strings and hardwiring them directly to the relay switches. Instead, I purchased a couple of 2-plug wall sockets to install into an electrical box and hardwired leads from those to the relay switches. The result is a portable box that can have lights (or other electrical appliances) installed and removed quite easily. While I could have easily crammed everything into a smaller box, the four-socket box afforded me a welcome amount of room in which to work.

With everything wired up and tested for faults, I connected my Arduino board to the relay switch and loaded it up with a sketch timed to match "Joy to the World." The code for which I borrowed from an Instructable which demonstrated how to build an 8-channel relay board from scratch. (Thanks, dany32412!) Despite only running a 4-channel relay system, the results were quite fantastic, as you can see in the video above when I plugged in some actual light strings to the system.

Hooked up to lights outside.

The cost to build my system? Just under twenty-six dollars in total. There are probably cheaper ways to have built the same thing, but I deemed it an acceptable expenditure, especially considering how I needed all of the parts for my next project.

The final product.

[Before attempting to replicate my project, be sure to know what you are doing before working with live power circuits. Serious harm, damage and/or death can occur when safety steps are not observed. Be warned that the end result of my work was in no way water- or environment-proof and was only ever installed outdoors for brief periods of time for demonstration purposes only.]