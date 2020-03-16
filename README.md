# Analog-Discovery-Addon
Combined BNC Adapter and Impedance Analyzer board for Analog Discovery


This project was designed using Altium Circuit maker. 

[Link to Circuit Maker Workspace](https://workspace.circuitmaker.com/Projects/Details/Yuri-Yuri/Analog-Discovery-Addon)

## Description

### BNC Adapter
Having BNC connectors on Analog discovery makes a ton of sense, it is a scope after all. For a long time I was using the male headers for everthing, it was a mess. The 14bit resolution on Analog Discovery can do things that my actuall bench scope can never dream of. Both oscilloscope chanells have AC/DC coupling options as well as 50ohm support.


After probe compensation using a 1KHz square wave the signal integrity improved so much in comparision to wires flying everywhere. You do lose the differential capability of scope channels when using this design, the oscilloscope negative channels are connected to Analog discovery ground.

### Impedance Analyzer 
Now that Digilent has Impedance Analyzer feature on waveforms it only makes sense to design hardware to go along with it. :-) 


This is based on the following block diagram, thanks to digilent. Image taken from this [Link](https://workspace.circuitmaker.com/Projects/Details/Yuri-Yuri/Analog-Discovery-Addon)

![alt text](https://github.com/adithyayuri/Analog-Discovery-Addon/blob/master/images/block-diagram.jpg "PCB TOP")


Digilent also has a [board](https://store.digilentinc.com/impedance-analyzer-for-analog-discovery/) that is made for inpedance analysis, it uses relays to switch between different reference resistors. But I wanted something that is simple so I just used bunch of jumpers to switch between different reference resistors. If you are planning to build this use good resistors, they need to have tolerance under 1%. 


### PCB Manufacturing

All the design constrains are made in accordance to [design capabilities](https://jlcpcb.com/capabilities/Capabilities) of JLCPCB. If you want to get this manufactured by someone else then you may need to make changes to the layout. I ordered my PCBs in matte  black(obviously). The price was unbeatable 10 units of my PCB for 2$, I was skeptical till the day someone knocked on my door.

![alt text](https://github.com/adithyayuri/Analog-Discovery-Addon/blob/master/images/jlc_order.png "Order page")

The PCB's I got were very well made, the matte black solder mask was gorgeous and silk screen was very clear (probably LPI-Liquid Photo Imaging process).

### Why make this when you can buy both?
I wanted to try using CircuitMaker so I made this to mainly to check out Altium's Circuit Maker and JLCPCB. I you want, you can buy BNC adapter for 20$ and Impedance analyzer for 22$ plus shipping(To asia it was 50$) on Digilent. Prices may change, check the below lins for product pages.

 - [BNC Adapter](https://store.digilentinc.com/bnc-adapter-for-analog-discovery/)
 - [Impedance Analyzer](https://store.digilentinc.com/impedance-analyzer-for-analog-discovery/)

I spent 2$ for 10pcs on PCB, and additional 11$ to populate 2 PCBs with parts. So to get two units working the __total cost is 13$__ including shipping.

## Images
### PCB Top
![alt text](https://github.com/adithyayuri/Analog-Discovery-Addon/blob/master/images/front.jpg "PCB TOP")
### PCB Top at an angle
![alt text](https://github.com/adithyayuri/Analog-Discovery-Addon/blob/master/images/front-angle.jpg "PCB Top at an angle")
### PCB Image on CircuitMaker
![alt text](https://github.com/adithyayuri/Analog-Discovery-Addon/blob/master/images/board_layers.png "PCB Top at an angle")
