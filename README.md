# Sliverflame, Propulsively Landing Model Rocket Using TVC
<img width="1200" height="400" alt="image" src="https://github.com/user-attachments/assets/36afb56f-49d5-41ad-922f-0e3160d4698b" />

## What is this?
Sliverflame is an active-stability model rocket designed to achieve vertical, propulsive landings using standard hobby rocket motors. This project is inspired by BPS space, when he landed his model rocket, Scout F. Additionally, I am doing this for stardance(stardance.hackclub.com/).


## How does it work?
1. Dual-Motors config, The rocket engine mount holds two motors sequentially. The upper landing motor is securely housed completely inside the body tube. The lower ascent motor sits partially inserted (~5mm) into the bottom of the tube.
2. Thrust based seperation, Once the ascent motor burns out, the top landing motor is ignited and it pushes the ascent motor in a different direction and then immediately the rocket stabilizes.

## Progress
I have finished design for all of the parts I just need to also 3D print them and I also with the budget of about $600 I can also laser cut landing legs. I am using PETG for the TVC gimbal and for the rest I am using regular PLA.

## Hardware
Look into the files for the parts in this directory or you can check it out in onshape: https://cad.onshape.com/documents/642eb1595bbfbb88e3413de9/w/294c2c178315e1ad00baf07d/e/72f61137f22d9a471da72dad.

Also I didn't go with a PCB because it was like $308 and it is way cheaper to just wire everything physically with wires instead on a PCB. But if you do want to check out the PCB it's in Kicad/ and gerbers.zip in Production/

<img width="303" height="404" alt="image" src="https://github.com/user-attachments/assets/a768bba0-49cc-4ca7-9880-d1e85370856e" />

Here is a shorted BOM list you can also check out the longer one in Rocket_BOM.csv:

| **Item / Category** | **Cost** | **Source** |
| :--- | :--- | :--- |
| **Estes F15 Rocket Motors (8-pack)** | $110.00 | Local Hobby Store |
| **SPARKHOBBY ES3352 Servos** | $48.28 | Amazon |
| **Custom Laser Cut Throttle Arms** | $32.66 | SendCutSend |
| **HOOVO 2S Shorty Lipo Batteries (2-pack)** | $34.43 | Amazon |
| **UHT Carbon Fiber Rods** | $25.69 | Amazon |
| **Avionics & Electronics** (ESP32-S3, MPU6050, BMP280, MOSFETs, UBECs) | $96.82 | Amazon |
| **Hardware & Miscellaneous** (Filament, Connectors, Wires, Fuses, Bag, Charger) | $162.93 | Amazon |
| **Structural Consumables** (Nichrome wire, Kraft paper, Rods, Glue, Bands) | $37.45 | Amazon |
| **Total** | **$548.26** | |

## Software
/Production/Software/ for all the software on the rocket. This rocket will be using Arduino IDE to program it. More info will come when I finish the software. My plan for the software is when the computer turns on it goes into a waiting loop and waits until my launch controller(which is also an ESP32) sends a signal to arm the rocket. The rocket then enters in a arm loop. it waits for the launch button to be pressed at the same time as the arm button, once it does it sends ignition to the first rocket motor, and when there is acceleration spike, it changes the variable motor1igntiontrue and then, It enters a Flight Loop. In the Flight loop it will use some math and the IMU gyroscope data, to see if the rocket is about to tilt over, if it is change the TVC orienatation to an opposite of the direction it's falling for a slight bit to get it back to stable, continuing to do those readjustments until the first motor burns out. It check's if the rocket is fine like if it crashed or if something else happened if did it will abort the flight and just fall (not that high). For the landing part is that it will ignite the top motor (landing motor) to push out the ascent motor and the TVC mount to angle one direction for just a bit and then re-stabilize immediately. Final part is just using the TVC loop and once it almost reaches the ground, throttle the motor (or also throttle it at the spike of the burn to prevent the rocket from going up). And finally then deploy landing legs via the nichrome wire and rubber band by burning it and then landing (hopefully).
 
## Safety Stuff
Since the rocket motor inside the tube can melt the TVC_Tube I am going to add some kraft paper inside so even if the exhaust touches inside the tube it will actually burn the paper and the throttle arms are made from Steel 1008 so I think its good. Additionally, I added software and hardware arming for the rocket motor, and I have to press both the Launch and Arm button to launch, so there is no way for me to accidentantly to ignite it.  

You can use this project however you'd like.
