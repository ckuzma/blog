#### 22.03.2020
### Ported Code for RGB Wall Display Board, Wired Up Buttons

![buttons](media/rgb_board_mk2/017_buttons.jpg)

As I fast approach the point of permanently encapsulating a microcontroller into my LED board, I decided to do some tests to see if I could utilize the [FastLED](https://github.com/FastLED/FastLED) Arduino library running on a NodeMCU v0.9 board.  The desire to do so was based on the number of existing projects that use this library, thereby giving me a lot more examples on which to base my own visualization code.  (Or, temporarily, to simply use another's code while I focus on finishing the assembly of my project.)

However my attempts to control my WS2812b LEDs was unsuccessful using FastLED and I wound up using the [Adafruit NeoMatrix](https://github.com/adafruit/Adafruit_NeoMatrix) library instead, just as I did with my [original light board](https://github.com/ckuzma/blog/blob/master/posts/2017/2017-12-30-rgb-led-matrix-board-litebrite.md) ([code](https://github.com/ckuzma/nodemcu-as-arduino/tree/master/Sketches/LED%20Board)).  Thankfully, Adafruit's libraries also enjoy a great deal of employment by other Arduino developers.  And seeing as one of the original goals of this project was to properly open-source [the original project that had caught my eye](https://github.com/ckuzma/blog/blob/master/posts/2020/2020-02-05-rgb-wall-display-board-part-1.md), this is probably for the best.

I also found some time this weekend to solder some wire leads to the buttons I'm hoping to use in my project.  As you can tell from the above photo things got a little messy, but the buttons seem to work just fine and the wires themselves will be hidden inside the project anyway.