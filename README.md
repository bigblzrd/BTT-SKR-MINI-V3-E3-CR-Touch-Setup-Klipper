# BTT SKR MINI V3 E3 - CR Touch Setup (Klipper)

If you've found yourself here then I can only assume you're incredibly frustrated and wanting to give up. But DON'T because this guide will *hopefully* get you up and running. 

I'll try and keep this short and sweet!

(I'm using an Ender 3 V2 Neo but it *should* be the same for others.)

## Pinout

For reference, this is the CR Touch pinout and as you can imagine it'll be quite important. 

Please note: It makes absolutely no sense but trust me - 

![image](https://github.com/bigblzrd/Test/assets/134751053/bdfc14af-ebee-4d91-804d-8f878976d260) WHITE = Ground  
![image](https://github.com/bigblzrd/Test/assets/134751053/ae81bf73-2e20-4853-910b-97768a0c0aa8) RED = Ground  
![image](https://github.com/bigblzrd/Test/assets/134751053/81d33615-8863-4045-9bef-6a150d0e4c70) BLACK = 5V  
![image](https://github.com/bigblzrd/Test/assets/134751053/99817f0d-75d4-4bd2-962d-2ec681b77b37) YELLOW = Servo  
![image](https://github.com/bigblzrd/Test/assets/134751053/aec8d95c-e2fb-4f8d-9b39-88514fd66363) BLUE = Signal  

## Wiring

For the CR Touch to work we need to do a couple of things. Firstly you'll need a single JST-XH 2 pin connector, these can be found in packs quite easily on Amazon or Aliexpress.  
Secondly we need to unpin some of the wires on the CR Touch connector but dont worry, this should be relatively easy with some patience and a... tooth pick? Theres a lot of guides on unpinning these kind've connectors so you should be good.

### Z Endstop Connector

For this we'll separate the 2 wires for the JST-XH connector -

![image](https://github.com/bigblzrd/Test/assets/134751053/ae81bf73-2e20-4853-910b-97768a0c0aa8) RED = Ground  
![image](https://github.com/bigblzrd/Test/assets/134751053/aec8d95c-e2fb-4f8d-9b39-88514fd66363) BLUE = Signal   

Make sure the the RED wire is on the left and the BLUE is on the right when plugged in, like so -

![image](https://github.com/bigblzrd/Test/assets/134751053/5906806f-da23-4877-9fde-4e0307c318fd)

### Main Connector

Now for this we need to rearrange the remaining 3 wires.

![image](https://github.com/bigblzrd/Test/assets/134751053/99817f0d-75d4-4bd2-962d-2ec681b77b37) YELLOW = Servo  
![image](https://github.com/bigblzrd/Test/assets/134751053/81d33615-8863-4045-9bef-6a150d0e4c70) BLACK = 5V  
![image](https://github.com/bigblzrd/Test/assets/134751053/bdfc14af-ebee-4d91-804d-8f878976d260) WHITE = Ground  

Here's how they need to be arranged, when plugged in it should look like this -

![image](https://github.com/bigblzrd/Test/assets/134751053/5817747a-3973-4325-8966-e3ab23d1e46c)

When finished with both connectors it should look *EXACTLY* like this.

![image](https://github.com/bigblzrd/Test/assets/134751053/b3f6b577-54ac-4a1a-b85a-5b16f2473a81)


## Configuration

Finally we need to change/add a couple of things in the Klipper printer.cfg file.  

  
I've attached files for the relevant sections that need changing - 

https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/blob/main/CR%20Touch%20Config  

https://github.com/bigblzrd/BTT-SKR-MINI-V3-E3---CR-Touch-Setup-Klipper-/blob/main/Stepper%20Z%20Config  

