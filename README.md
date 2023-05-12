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

### Current:

#### Supplier
 - Supplier supplies Part
 - Supplier can supply Part (shows the difference between possibility to supply and actually supplying)


#### Assembly
 - Assembly has Part
 - Assembly has Assembly
 - Assembly is specified by Specification
 - Assembly is instructed by Instruction


#### Product
 - Product has Assembly
 - Product has Part


#### Specification
 - Specification specifies Part
 - Specification specifies Assembly
 - Specification specifies Product


#### Instruction
 - Instruction instructs Part
 - Instruction instructs Assembly
 - Instruction instructs Product


### Future:

#### Supplier
 - Supplier supplies Assembly
 - Supplier can supply Assembly (shows the difference between possibility to supply and actually supplying)


#### Person
 - Person assembles Part
 - Person assembles Assembly


#### Product
 - Product is sold to Client
 - Product is packaged with Packaging


#### Part
 - Part could be in Assembly (shows possible re-use use case)
 - Part could be in Product


#### Assembly
 - Assembly could be in Product

