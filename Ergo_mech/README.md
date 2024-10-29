# Custom ergonomic mechanical design


This is a custom design for mechanical parts matching the OS3M PCB. It has some nice added features:
* Ergonomic shape 
* Made to have a 2 mm soft insert
* Compartment for adding dead weight
* Designed to have up to four 6x6x5 mm SPST switches that can be connected to the PCB (Note: firmware is not yet ready for this)
* The bottom has recesses for gluing in rubber "feet"

*Credits: To save some time I borrowed a couple of profiles from Thingiverse #4772023 (handrest for 3dConnexion) by SenJos**

## Re-used parts

The folowing parts are re-used from the original design or other forks:
### Knob

![](HEIA_knob.png?raw=true)

You may use the upstream knob, but if you want to use the "cap" part, it's only tested with the knob from the fork https://github.com/Overlord6644/os3m-hardware, also included here in a slightly modified version. 

Regarding the 'target' (copper pieces) matching this knob, see below.

### Stem 
Use the upstream part in the 3MF folder
### Flexure 
You can use anyone you like

I have copied the reinforced version by lpurdy into the 3MF folder

## Unique parts

### Base and handrest

Exported in two versions:

   * four-button
		
		![](base_and_handrest_4_buttons.png?raw=true)
	
   * one-button
		
		![](base_and_handrest_1_buttons.png?raw=true)
	 
Printing tips:

  * If you print it flat, you will get very noticeable layers. The effect can be reduced by reducing layer thickness as much as you have time to wait. You can of course also sand and polish or paint the surface. 20% lightning infill worked fine for me.
  * You get a better top surface by printing it lying on its side, but then use an infill that also supports sideways (not lightning). Some extra supports to keep it from tilting is adviced if you are able to add it.

### 3buttons
![](3buttons.png?raw=true)

This part is not used if you select the one-button version of the base 

May need a countersunk M3 screw to stay in place

Printing tips:

   * For best strength, print it lying on its side

### 1button
 
![](1button.png?raw=true)

This is the thumb button

It sould have a press-fit tolerance, but you may need to adjust it slightly depending on your print tolerances

Printing tips:

* For best strength, print it lying on its side

### cap
![](cap.png?raw=true)
	
THis is an optional part, its function is to better hide the PCB and screws

Only tested together with the knob included here. If you want one matching the upstream knob, add a request.

Printing tips:
* This should ideally also be printed lying on its side, but I haven't been successful yet.

### bottom lid 
 ![](bottom.png?raw=true)

An optional part, only needed if you want to fill the bottom compartment with something to increase the weight.
Must be fastened with four M3 screws

### foam_stencil
![](foam_stensil.png?raw=true)

This is a flattened and slightly shrunk version of the foam insert. 

Print it and use as a cutting stencil on 2 mm foam, leather, cork or other soft material.

Note: The holes were added just to save material and print time.

### custom_target
![](custom_target.png?raw=true)

This is a paper stencil for the target designed by https://github.com/lpurdy01/os3m_target_testing and matches the knob included here

Print the PDF on paper and use as stencil to cut copper sheet metal (1 mm thickness is fine). 


## Adding switches

The switches shall be 6x6x5mm, no bracket, either through-hole or SMT. 

Cut off the legs on one side and solder wires on the other.

Make sure you remove all printing supports on the base.

Route the wires, place the switches and attach the "button" parts. 

![](3_switches_mounted.png?raw=true)

(To be continued)