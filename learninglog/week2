## LEARNING LOG WEEK 2

This week I learnt some more about resistors (like how to tell the value by the coloured stripes) and that it's possible to use the breadboard without connecting it to my laptop and Ardurino. We just plugged in a battery! (Idk why that surprised me so much haha)
We also talked about Voltages, Currents and Resistance which I already hated in physics and definetly have to look in again until next week (sigh). 
We then talked about the diffrences of a series circuit vs a parralel ciruit, which I actually remeber really well from physics class (yay!), so no need to revise.
Additionally we built a traffic light system and I'm very proud to have come up with the code myself and it working really well!
The last thing we did included an RGB LED (super cool as well) and learning constants and setRGB( ). Here I messed up once by putting my power board in the wrong way so switching up + and - (whoops), but otherwise everything worked well.


### Notes
(also avalible on my [Notion](https://app.notion.com/p/Week-2-Oct-20-RGB-and-Resistors-3ff1a46c8a6e80abac8be53e75df7d27?source=copy_link))

- THT = Through Hole Technology
- SMD = Surface Mount Device
- LED = Lightning Emitting Devive
- Resistor Colour Code: used to represent value

- Breadboard: all power rails are connected top to bottom, in the main field the terminal strips  are connected horizonatlly

- to power the breadboard Ardurino, a power module or battery can be used
- variation in circut (chaning the wires (5V instead of GND)) causes the powerflow to change so either the LED or the yellow light on the controller board have power which causes the synchronised blinking
- GND (Ground):
    - the circuits common ground, acting as a zero volt refrence and return path for current
    - in a direct current (DC) circuit, the negative (-) terminal is often designated to the ground

| Voltage | V | Volt, V |
| Current | I | Amp, A |
| Resistance  | R | Ohm, **Ω** |
- 220 **Ω** resistor for LED for current limiting <15mA
- direct current (eg laptop, smartphone) vs alternating current (big househould machines, eg washing machine) bc it is more practical in long distance power transmission but less safe and harder to change voltage
- common voltages:
    - for microcontrollers 5V (standard), 3.3V (saving energy)
    - 9V (final project)
    - 12V (highest we can go here while being safe)


- use a series circuit when you need components to divide voltage/sharing current
- use a parralel circut when you need every device to recieve the full source volate + it’s the  safer scenario bc when one thing breaks the rest still runs
- Green LEDs are less bright (bc of diffrent forward voltage), to make it even use a smaller resistor on it
- RGB LED: needs 3 resistors bc they always go between the + and the LED itself, the second/longest leg is minus, the other ones are R,G and B
- setRGB( ) allows us to modify the RGB LED to diffrent colours by using the function analogWrite( ) 255 is max brightness, 0 is minimum
