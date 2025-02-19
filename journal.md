# firstly,

This 3D printer has been made possible by Hack Club and the awesome Alex Ren. Let's give them a hand! 👏👏👏

Made by: @padimo
Repository link: https://github.com/Omegon0/Infill  
Total hours so far: 0

 - ✅  I have a 3D printer

# About the Padimo Mini
I have too many ideas and not enough time near my printer. 
Target speed: 40 mm/s
Target print volume: 50mm x 50mm x 60mm
Materials: PLA

# day 1 (2/15/25)
Coming up with ideas to maximize print volume inside of my 10 by 10 by 10 constraints.
First off, the PMU has to be detatchable. There's no way it will fit otherwise.
Second, the extruder is going to be very big relative to the printer itself. So that's going to be detatchable too. 
X and Y will need pulleys and Z will need a screw, it's unavoidable.
the screen can cover one face so that's fine. but it means that i'll need a touchscreen because rotary encoders are too big, so Adafruit ILI9341 touchscreen with microSD socket? 
https://www.adafruit.com/product/1770
now i need a mainboard that uses SPI for both the card and the screen. and is 100mm or less. not happening

# day 2 (2/17/25, 3 hours)
I found someone who is making a battery powered printer https://infill.hackclub.com/printers/volt-core/
I think I need a BOM which means research so here's what I found
- PMU (tomorrow)
- main board
	- https://www.amazon.com/BIGTREETECH-Controller-Raspberry-Printing-Motherboard/dp/B09MYKL9MP
- X axis
	- belt and https://kb-3d.com/store/stepper-motors-servos/67-ldo-stepper-motor-nema-8-20sth38-0604a-1666451386927.html?gQT=2
- Y axis
	- belt and https://kb-3d.com/store/stepper-motors-servos/67-ldo-stepper-motor-nema-8-20sth38-0604a-1666451386927.html?gQT=2
- Z axis
	- https://www.amazon.com/Stepper-Linear-Actuator-Engraving-Machine/dp/B09BZDSY7V/
	- bed not heated because I will use PLA and blue painter's tape on top of aluminum
- extruder
	- hotend
	- extruder motor

By now I've realized why people don't make tiny FDM printers. None of the small steppers have enough torque. 
And I'd need 300 Wh to run a longish print. Car battery too big

# day 3 (2/18/25, 4 hours)
I forgot to push yesterday's entry oops
Also I'm changing the dimensions and I'm making it a bed slinger because that's easier
New dimensions: 80mm by 120mm by 120mm (80 is X or Y, not Z)
I am making an actual BOM file now and starting to fusion it because I definitely won't have enough space (i might if I do this right)
I thought about making it a bed slinger then I discovered 10mm aluminum extrusions exist and I can make a flying gantry printer
Then I realized that CoreXY kinematics exist and [this](https://user-images.githubusercontent.com/44207097/47033555-7474f180-d175-11e8-912e-9c43061537b0.png) uses the least bearings so that's what i'm going with

Found 10mm by 10mm aluminum extrusions, [these T slot nuts](https://www.amazon.com/MakerBeam-pieces-T-slot-nuts-screws/dp/B016OJNLJ2), [these corner cubes](https://www.amazon.com/MakerBeam-Corner-Cube-Black-pcs/dp/B00OWGOMG6/) (but i'm not using the corner cubes because reprap)

I'll fusion tomorrow I promise
