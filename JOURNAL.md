---
title: "Silverflame - TVC propulsively landing rocket"
github: "https://github.com/CloudStas/Sliverflame-TVC_Rocket"
description: "A rocket that uses TVC(Thrust Vector Control) with throttle arms to land propulsively like the falcon 9 rocket."
created_at: "2026-08-18"
total_time: "65h 28m"
---

# August 25, 2026

There are a lot of parts for a Propulsively Landing Model Rocket, and I finished 1 one them which is Designing the TVC Mount. TVC or Thrust Vector Control is for gimbaling the rocket motor so the rocket can go upward straight. The Mount can also hold 2 motors one for ascent and another one for landing. Once the Landing motor burns out it literally just gets jettisoned and it falls out as the landing motor inside the tube ignites and the throttle arms are originally open but the throttle arms can be commanded by the flight computer to throttle down when needed. When the rocket gets closer to the ground it can throttle down more so it can become slower and slower until the legs touchdown on the ground. Right now I am currently designing the flight computer which is my first PCB and then I will make a mount for the rocket to hold the computer and the battery. After the Flight Computer is done I will work on the Reaction Wheel to Stabilize the rocket's roll, and the airframe of the rocket which is simple, it's just cardboard. And the final hardware design step is to design the landing legs which will be most likely to be made out of carbon fiber with a toy dampener. The way the legs work is kind of simple, they just have a nichrome wire on top of the legs, when the electrical current gets sent thru the wire it burns up and the legs can get out and click in so they are ready for impact. My Mount btw uses plastic + ceramic throttle arms and 4x Genuine MG90s servo's. That said, Here is my TVC Mount: You can also check out the project on Github: https://github.com/CloudStas/Propulsively-Landing-Model-Rocket

![](https://fabricate.hackclub-assets.com/de959ed7c66ca4073d8269a253fac39c56968706f7ff4e438d839c34d438e4a9/image-png/image.png)

**Total time spent: 9h 58m**

# August 30, 2026

Right now I am almost finished with the flight computer I spent most of the time fixing issues. And once I am finished I will post the BOM and add it to my github repo. Here are some features of the flight computer: The main CPU will be the ESP32-S3 and it will power 4x DC motors, 2x of them for YAW and PITCH and 2x more will be for the throttle arms, and lastly a dc motor for a reaction wheel to stabilize the rocket's roll.

![](https://fabricate.hackclub-assets.com/2703b4d3421e6a4bf06cb6035a0d72b91ced1b07cc8914f47da5f43da38f76c0/image-png/image.png)

**Total time spent: 11h**

# September 8, 2026

I was designing my PCB but I decided to not make my own pcb and instead just use a Pi zero 2w and a teensy 4.1 with seperate igniters and servo/motor power connections. So now I am going to be designing an avionics bay in onshape to hold the computers and all the electronics. Edit: I am going to finish the pcb I am just going to finish the rocket design first.

![](https://fabricate.hackclub-assets.com/4eee224b846904a255baef2def20668c95ce291797e9f99961021614f508cfc8/image-png/image.png)

**Total time spent: 7h 54m**

# September 10, 2026

I am redesigning the TVC mount with a better one so it can move better on it's X/Y axis and also to be smaller. I still need to do the throttle arms and before that also need to figure out how to make it smaller to fit in something like a 74mm OD(Outer Diameter) tube or similar.

![](https://fabricate.hackclub-assets.com/f22c0839ecaec57bac98c049419a4567a3ffab3f190731c05769efba98b6af62/image-png/image.png)

**Total time spent: 7h 44m**

# September 16, 2026

I finally finished the TVC mount with throttle arms. And it supports 2 rocket motors and it can gimbal in all directions 5 degrees, I am basically done with the one of the hart parts. Up next I am going to redesign the flight computer PCB.

![](https://fabricate.hackclub-assets.com/145e1d87105bd1758bd85456f092b9270a22e745a11487a55798f61a3763030b/image-png/image.png)

**Total time spent: 10h 36m**

# September 18, 2026

I thought of finishing the PCB but realized that it would take a few weeks for it to be made so instead i decided to daisy chain everything and I also designed an Avionics Bay that holds 2 computers(1x Raspberry Pi 3 Model A+ that is connected to a camera, and 1x ESP32-S3) and the ESP can send signals to ignite rocket engines or deploy landing legs. I also made a spreadsheet for all the parts and here is how the Avionics Bay and the BOM(Bill Of Materials) looks like: Also here is the BOM Link: https://docs.google.com/spreadsheets/d/1w17DnCs4J0WBasmAesTz5ANlNJR9XYsVwglhH3W97UI/edit?pli=1&gid=0#gid=0 Total Cost for the Electronics is The materials without 3d printing which is the final step is $482.35, I am going to later try to optimize the cost but for now I need to finish designing the rocket and then I will.

![](https://fabricate.hackclub-assets.com/bac345a20660aedbf1bad5fa3f17f456e2aa4b6920bd03b3a70422d963fc49c7/image-png/image.png)

![](https://fabricate.hackclub-assets.com/a6d41a7d0d22cac3f289de1f3e1a89c84b247a561b38093f26e704e3acd6a1f6/image-png/image.png)

**Total time spent: 4h 46m**

# September 28, 2026

I am basically finished with the Landing legs for my TVC rocket and I just have to finish my PCB since the deadline got expanded to oct 31st so I have enough time. I might make a reaction wheel since I have enough time. I might also make a reaction wheel for stabilizing rocket's roll. I am excited for launch.

![](https://fabricate.hackclub-assets.com/41e49c5d56a4098e6a185489498ab304b1b1e499e17eda0cdfff0533d292fea0/image-png/image.png)

**Total time spent: 6h 46m**

# October 2, 2026

I finally finished my PCB costs about $30 on JLCPCB: this pcb has an ESP32 for control and powers from a 2s lipo battery 2200mah and powers 4x KST x08 v6 servos for XY control and throttle control and a usb port for debugging and 2x Igniters for 2x Estes F15 motors and 1x for releasing landing legs, almost done with the rocket.

![](https://fabricate.hackclub-assets.com/1c5dd278dc3a9242cbdd9d3b0c86cce0ca0d7efe1168c1191af4036f8faedf70/image-png/image.png)

![](https://fabricate.hackclub-assets.com/8b0935a3c3a7e7aa44e4e504c3fbaf590dce95731c5206b1b24463beba0f465c/image-png/image.png)

**Total time spent: 2h 43m**

# October 10, 2026

I have finished on the rocket and I submitted for funding I don't really know how to make logos so I just threw up something together, and I guess it's fine. I also made the BOM (Bill Of materials) you can also check out my project on https://github.com/CloudStas/Propulsively-Landing-Model-Rocket

![](https://fabricate.hackclub-assets.com/7c37fb7c599c22bf1a0a689d11f1e760418162e4ad8c2978e36c12cfe2b22c2a/image-png/image.png)

![](https://fabricate.hackclub-assets.com/28ce906fc27a2a77eb11df6316e2d4ba49b78f9b55a85c492cc40ab7389bac1a/image-png/image.png)

**Total time spent: 3h 57m**
