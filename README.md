# Sliverflame, Propulsively Landing Model Rocket Using TVC

## What is this?
Sliverflame is an active-stability model rocket designed to achieve vertical, propulsive landings using standard hobby rocket motors. This project is inspired by BPS space, when he landed his model rocket, Scout F. Additionally, I am doing this for stardance(stardance.hackclub.com/).

## How does it work?
1. Dual-Motors config, The rocket engine mount holds two motors sequentially. The upper landing motor is securely housed completely inside the body tube. The lower ascent motor sits partially inserted (~5mm) into the bottom of the tube.
2. Thrust based seperation, Once the ascent motor burns out, the top landing motor is ignited and it pushes the ascent motor in a different direction and then immediately the rocket stabilizes.

## Progress
I have finished design for all of the parts I just need to also 3D print them and I also with the budget of about $600 I can also laser cut landing legs. I am using PETG for the TVC gimbal and for the rest I am using regular PLA.

## Hardware
Look into the files for the parts in this directory or you can check it out in onshape: https://cad.onshape.com/documents/642eb1595bbfbb88e3413de9/w/294c2c178315e1ad00baf07d/e/72f61137f22d9a471da72dad.

| **Item / Category** | **Estimated Cost** | **Source** |
| :--- | :--- | :--- |
| **Estes F15 Rocket Motors (8-pack)** | $110.00 | some hobby store |
| **SPARKHOBBY ES3352 Servos** | $48.28 | Amazon |
| **Custom Laser Cut Throttle Arms** | $32.66 | SendCutSend |
| **HOOVO 2S Shorty Lipo Batteries (2-pack)** | $34.43 | Amazon |
| **UHT Carbon Fiber Rods** | $25.69 | Amazon |
| **Avionics & Electronics** (ESP32-S3, MPU6050, BMP280, MOSFETs, UBEC) | $81.32 | Amazon |
| **Hardware & Miscellaneous** (Filament, Connectors, Wires, Fuses, Bag) | $105.90 | Amazon |
| **Structural Consumables** (Nichrome wire, Kraft paper, Rods, Glue, Bands) | $40.44 | Amazon |
| **Total** | **$538.27** | |

## Software
software/ for all the software on the rocket. This rocket will be using Arduino IDE and probably something like simulink for simulating the rocket landing. More info will come when I finish the software.

## Safety Stuff
Since the rocket motor inside the tube can melt the TVC_Tube I am going to add some kraft paper inside so even if the exhaust touches inside the tube it will actually burn the paper and the throttle arms are made from Steel 1008 so I think its good.

You can use this project however you'd like.
