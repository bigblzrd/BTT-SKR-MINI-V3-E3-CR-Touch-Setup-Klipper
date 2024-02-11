# BTT SKR MINI V3 E3 - CR Touch Setup (Klipper)

If you've found yourself here then I can only assume you're incredibly frustrated and wanting to give up. But DON'T because this guide will *hopefully* get you up and running. 

I'll try and keep this short and sweet!

(I'm using an Ender 3 V2 Neo but it *should* be the same for others.)

## Pinout

For reference, this is the CR Touch pinout and as you can imagine it'll be quite important. 

Please note: It makes absolutely no sense but trust me - 

![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/f4c2c843-7979-4acc-a02b-c74af969470c) WHITE = Ground  
![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/58308e43-35c3-4770-810c-da64e46bb791) RED = Ground  
![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/4ea4303e-fda3-46a3-aafb-e5b9d160b6a9) BLACK = 5V  
![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/f3c3e8c4-372b-4b67-a891-1c52cd19b874) YELLOW = Servo  
![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/c0b31637-9718-47fb-a959-56ccca1bc30f) BLUE = Signal  

## Wiring

For the CR Touch to work we need to do a couple of things. Firstly you'll need a single JST-XH 2 pin connector, these can be found in packs quite easily on Amazon or Aliexpress.  
Secondly we need to unpin some of the wires on the CR Touch connector but don't worry, this should be relatively easy with some patience and a... tooth pick? There's a lot of guides on unpinning these kind've connectors so you should be good.

### Z Endstop Connector

For this we'll separate the 2 wires for the JST-XH connector -  

![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/58308e43-35c3-4770-810c-da64e46bb791) RED = Ground  
![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/c0b31637-9718-47fb-a959-56ccca1bc30f) BLUE = Signal  

Make sure the the RED wire is on the left and the BLUE is on the right when plugged in, like so -  

![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/6133e1f3-6746-40fc-8393-00f1cf997c66)


### Main Connector

Now for this we need to rearrange the remaining 3 wires.

![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/f3c3e8c4-372b-4b67-a891-1c52cd19b874) YELLOW = Servo  
![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/4ea4303e-fda3-46a3-aafb-e5b9d160b6a9) BLACK = 5V  
![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/f4c2c843-7979-4acc-a02b-c74af969470c) WHITE = Ground  

Here's how they need to be arranged, when plugged in it should look like this -  

![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/32d6e3dc-be6e-4973-8480-49eb9267ca42)


When finished with both connectors it should look *EXACTLY* like this.

![image](https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/assets/134751053/8b8465d2-3b7f-42b4-85e0-e8de64ae6382)



## Configuration

Finally we need to change/add a couple of things in the Klipper printer.cfg file.  

  
I've attached files for the relevant sections that need changing - 

CR Touch:
https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/blob/main/CR%20Touch%20Config  

Stepper Z:
https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/blob/main/Stepper%20Z%20Config  

