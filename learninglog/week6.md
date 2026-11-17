## LEARNING LOG WEEK 6

This Tuesday morning we used the Stepper Motor for the first time. Another very useful gadget. I found it especially fun in combinantion with the Touch Sensor (so cool). 
Unfortunatly my battery didn't work that well, which made me kinda insecure bc it didn't work for a while and I thought I was doing something wrong. Luckily I could just use my Ardurino as power source.
For exercise 3 I had some help from ChatGPT: basically did whatever I could and then send my unfinised to to ChatGPT to get it finished, but I think I was close do doing it almost alone (like 90%).


(also avalible on my [Notion](https://app.notion.com/p/Week-6-Nov-17-Stepper-Motor-41b1a46c8a6e800a8927e0044102cbd6?source=copy_link))

- Stepper Motor:
    - very precise control of positions
    - large torque at low speed
    - BUT tricky to use (need a matching driver + different code for diffrent specs)
    - needs extrernal power supply, usually can’t do it with just Ardurino
- Works bc of the change of electro magnetic field
- Red cable is 5V
- Libaries: cheapStepper, Stepper (Ardurino default) & AccelStepper (finer control of speed accelaration and position)
- RPM: revolutions per minute: can vary based on different stepper motors
(and the settings on the motor driver)
- Stepper motors are called stepper motors because they
move in 'steps'
- moveDegree() is a function that calculates between
steps and degrees to make it easier
- Blocking & Non-blocking Functions:
    - An Arduino sketch "pauses" during blocking functions
    such as: moveDegrees() , move() & moveTo()
    - If you want to be able to control other components while a stepper is moving, use: newMoveDegrees() , newMove() & newMoveTo()
        - need to call stepper.run() in the loop
- Touch Sensor: no pullup/down neccesary


### Exercises

#### Exercise 1: moveDegrees()

<img width="2048" height="2731" alt="grafik" src="https://github.com/user-attachments/assets/63797597-2aaa-4818-988a-146f33a2d72f" />

**Challenges:**

- Change the value of moveDegrees() to some other
values and observe the steps → smaller value = smaller steps
- How to make the stepper tick like a second-hand on a clock? → stepper.moveDegrees (moveClockwise, 6); & delay (900) because the movement itself takes 100ms

#### Exercise 2: move() VS moveTo()

- defining the destination not position
- stepper.moveTo uses steps instead of degrees
- Challenge: How to switch back and for th with clockwise / counterclockwise direction? → change true to false (bool)

<img width="1530" height="996" alt="grafik" src="https://github.com/user-attachments/assets/a181bfa7-c1b5-4f2c-a59e-4e942a7ec926" />


#### Exercise 3:  Move and more
 <img width="2048" height="2731" alt="grafik" src="https://github.com/user-attachments/assets/d22737a0-ae91-49b8-99e6-293b66e35eb8" />
 <img width="1335" height="981" alt="grafik" src="https://github.com/user-attachments/assets/e79c4436-a008-4d48-9485-4a75ea6f30cc" />

Next Step: Adding LEDs:
<img width="2048" height="2731" alt="grafik" src="https://github.com/user-attachments/assets/ef9125bb-3223-4714-862d-527f8c1f6392" />
<img width="1597" height="950" alt="grafik" src="https://github.com/user-attachments/assets/b5dbf46b-3c86-427e-ab21-72093e4dda15" />

Challenge: stepper.stop() cancels the current movement and resets the remaining steps so remove it from code and add return; 
<img width="665" height="249" alt="grafik" src="https://github.com/user-attachments/assets/bb059094-8abe-4ebb-84e1-b912f4adf2d5" />

