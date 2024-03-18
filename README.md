# Songs for playing on Arduino boards.

## Usage

Every code here should run on every arduino board without problems. The sketches rely solely on the tone() function from Arduino, so the sounds are all monophonic. On the bright side, **libraries are not required**.

If you want to compare the code with the original score, I try to group the notes in a measure as one line of ccode and the staves as groups of lines. However, in some cases notes will be tied together among measures or be dotted and this rule is broken.

## Hardware

Just connect an piezo to the board and you are good to go. Pin 3 is used in every sketch because some piezo speaker can be connected between it and the close GND pin without any wiring. You can use basically any pin, as long  as they can be used as digital pins (pins A6 and A7 of the Arduino Nano and mini are analog only). Just remember to assign the pin number to the `buzzer` variable. 

There are two kinds of piezo buzzers: active and passive. The active one that plays a specific pitch when powevered and is not good for this purpose. The passive kind functions like a speaker, reproducing the pitch you apply to it. You can test the piezo speaker with the "blink" example, the good piezo speaker will just click, while the other kind will play a pitch every other second.  

## Copyright

This was cloned from https://github.com/robsoncouto/arduino-songs/ all credit given to him.
