## LEARNING LOG WEEK 3

This week we got deeper into analogWrite() and also introduced analogRead().
We also worked with many new components such as the Tilt Switch, the Potentiometer and the Photoresistor. 
In general I found this week a lot more challenging than the previous ones. Exercises 1-3 were "understandable" for me and I could come up with the solution myself. However Exercise 4 was really hard for me and I could not figure it out myself, in retroperspective I understand it tho.
To my own surprise I actually enjoy the "building" and find a lot easier and more natural than the coding. 


### Notes
(also avalible on my [Notion](https://app.notion.com/p/Week-3-Oct-27-analogRead-Write-4061a46c8a6e80c2a21ceedec5147809?source=copy_link))
- analogWrite( ) - PWM (Pulse-Width Modulation)
    - pulse-width modulation, is a digital method of controlling analog power pyrapidly switching a signal on and off
    - 0-255 “translation”, mapping between 0v and 5v (8bits)
    - it’s a widely used technique in dimming LEDs, controlling motor speed, etc
- duty cycle: the promotion of "on-time" in each cycle

!grafik.png

- Oscilloscope: a device that measures voltages and displays it graphically
    - give pin and value (0-255):  (pinMode (OUTPUT) → setup and analogWrite → loop)
    - chaning the value / duty cycle creates a signal change displayed as bump → PMW
- Analog signals are continuous and vary smoothly over time
- Digital signals are discrete and usually represented by binar y
states (0 and 1)
- analog pins can also be used for digital output

!grafik.png

- reset button doesn’t delete the code, it just reruns it
- TX(transmit), RX(Receive) are reser ved for serial communication, usually we don't use these two pins, you can use these two pins as normal digital pins if no serial communication is needed
- 2-13: Digital I/O pins, ~ for PWM
- A0-5: Analog Input Pins
- VIN: to power the Arduino UNO (7-12V)
- Reset: does the same job as the reset button
- IOREF: Reference Voltage for all I/O pins, connected to 5v on Arduino UNO
- digitalWrite() / digitalRead()
HIGH - 5V
Low - 0V
→ Both Digital and Analog Pins
- Tilt Switch: a component that can detect the tilting of an object
    - cables are not connected
    - stable connection when upright so connected to the ground → 0
    - when it’s unstabe it’s not connected to anywhere → 1
    - cables create noise
    
    !grafik.png
    
- Serial Baud Rate
    - Serial baud rates are the number of signal changes per second in a serial communication channel
    - The specific rate must be matched between the transmitting and receiving devices for successful communication.
    - Most commonly used value for Arduino: 9600 bps
- INPUT_PULLUP
    - Ask Arduino to use internal pull-up resistors (resistors that connect to power internally)
    - Prevents Floating Pins: Without a pull-up or pull-down resistor, an unconnected pin "floats," picking up electrical noise and returning random, unstable HIGH or LOW values.
- AnalogRead()
    - An analog pin will give you a value between 0 and 1023,
    where 0 means 0V and 1023 means the maximum voltage
    possible (5V by default).
    - You can only use analogRead() on Analog pins
- ADC
    - An Arduino UNO contains a 10-bit, 6-channel analog todigital conver ter (ADC)
    - A device that conver ts an analog signal (voltage) into a
    digital value
    - You can set the AREF(Analog Reference) pin to sth lower than 5v for higher resolution for low voltage component
- Potentiometer (linear)
    - A potentiometer is an adjustable resistor
    - Most common use Case: Volume Adjustment
    - similar to a sound synthesiser
    - middle pin for output! others for power and ground (swap to chnage direction)
    - 1023 = 5V
    
    !grafik.png
    
- Volatage Divider:
    - series circuit
    
    !grafik.png
    
- Serial Read
- Photoresistor: also called a light-dependent resistor (LDR), is a light- sensitive variable resistor whose resistance decreases as the intensity of light hitting its surface increases


### Exercises

#### Exercise 1: Fade in/out a LED

!IMG_3017.heic

!Screenshot 2026-10-27 103159.png

#### Exercise 2: DigitalRead( )

!IMG_3018.heic

!Screenshot 2026-10-27 105505.png

!Screenshot 2026-10-27 111327.png

#### Exercise 3: AnalogRead( )

!IMG_3020.heic

!Screenshot 2026-10-27 114901.png

#### Exercise 4: Read input from Serial

skipped

#### Exercise 5: analogRead() with Photoresistor
<img width="2048" height="2731" alt="grafik" src="https://github.com/user-attachments/assets/2c1a074d-1369-4e9b-85f5-ed5fe776864e" />

<img width="1223" height="1010" alt="grafik" src="https://github.com/user-attachments/assets/3ef78117-e99b-4f62-8d4e-8493782004c1" />

<img width="1830" height="1014" alt="grafik" src="https://github.com/user-attachments/assets/b4ebe0b6-e25d-46a7-890b-9dfd81b3bfe8" />

