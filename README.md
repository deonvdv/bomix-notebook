# bomix-notebook
Bomix Notebook

## BOM

```
Bicycle
	Wheel
		Spokes
		Hub
		Rim
			Color
		Tire
		Valve
	Front Set
		Handlebar grip
		Front brake
		Fork
			Color
		Shifter
	Saddle Area
		Saddle
		Seat post
	Transmission
		Chain
		Chain Rings
		Rear brakes
		Cog set
		Rear Derailluer
		Front Derailleur
		Pedal
		Crank Arm
	Frame
		Frame
		Stem
		Head
			Color
```


## Relationships



### Supplier
 - Supplier supplies Part
 - Supplier supplies Assembly


### Person
 - Person assembles Part
 - Person assembles Assembly


### Assembly
 - Assembly is sourced from Supplier
 - Assembly belongs to Product
 - Assembly has Part
 - Assembly has Assembly
 - Assembly is assembled by Person
 - Assembly is specified by Specification
 - Assembly is instructed by Instruction


### Part
 - Part is assembled by Person
 - Part is sourced from Supplier
 - Part belongs to Product
 - Part belongs to Assembly
 - Part is specified by Specification
 - Part is instructed by Instruction


### Product
 - Product has Assembly
 - Product has Part
 - Product is specified by Specification
 - Product is instructed by Instruction


### Specification
 - Specification specifies Part
 - Specification specifies Assembly
 - Specification specifies Product


### Instruction
 - Instruction instructs Part
 - Instruction instructs Assembly
 - Instruction instructs Product
