# Custom ergonomic mechanical design


This is a custom design for mechanical parts matching the OS3M PCB. It has (in my view) some nice added features:
* Ergonomic shape 
* Made to have a 2 mm soft insert
* Compartment for adding dead weight
* Designed to have up to four 6x6x5 mm SPST switches that can be connected to the PCB (Note: firmware is not yet ready for this)
* The bottom has recesses for gluing in rubber "feet"

The design is made in Solid Edge Community Version, which is free so anyone should be able to extend the work if you like. Note that the files cannot (according to Siemens) be opened in the *commercial* version of Solid Edge. It's my first use of this tool so don't be suprised if you see that some features could have been done in a smarter way.

*Credits: To save some time I borrowed a couple of profiles from Thingiverse #4772023 (handrest for 3dConnexion) by SenJos. Other re-used but slightly modified items are the knob from the HEIA fork, the target from lpurdy and the stem from spoter368*

## Parts

### Knob

![](HEIA_knob.png?raw=true)

You may use the upstream knob, but if you want to use the "cap" part, it's only tested with the knob from the fork https://github.com/Overlord6644/os3m-hardware, also included here in a slightly modified version. 

Regarding the 'target' (copper pieces) matching this knob, see below.

### Stem 
You can use the upstream part, but a slightly modified version  - that gives a more tight fit with the Cap - is included here.

Printing tips:
Print upside down without supports.
For right-hand mouse: Same part

### Flexure 
You can use anyone you like.

The - in my opinion - best one for now is the reinforced version by lpurdy, which is copied into the Exports folder.

Printing tips:

* Supports are not needed.
* For right-hand mouse: Same part

### Base and handrest

Exported in two versions:

   * four-button
		
		![](base_and_handrest_4_buttons.png?raw=true)
	
   * one-button
		
		![](base_and_handrest_1_buttons.png?raw=true)
	 
Printing tips:

  * If you print it flat, you will get very noticeable layers. The effect can be reduced by reducing layer thickness as much as you have time to wait. You can of course also sand and polish or paint the surface. 20% lightning infill worked fine for me.
  * You get a better top surface by printing it lying on its side, but then use an infill that also supports sideways (not lightning). Some extra supports to keep it from tilting is adviced if you are able to add it. My best results have been with Cura's "tree" support.
  * For right-hand mouse: Mirror about Y-axis

### 3buttons
![](3buttons.png?raw=true)

This part is not used if you select the one-button version of the base 

May need a countersunk M3 screw to stay in place

Printing tips:

   * For best strength, print it lying on its side
   * For right-hand mouse: Mirror about Y-axis

### 1button
 
![](1button.png?raw=true)

This is the thumb button

It sould have a press-fit tolerance, but you may need to adjust it slightly depending on your print tolerances

Printing tips:

* For best strength, print it lying on its side
* For right-hand mouse: Mirror about Y-axis

### cap
![](cap.png?raw=true)
	
This is an optional part, its function is to better hide the PCB and screws, and to protect it from dust, food etc that might fall down.

Only tested together with the knob included here. If you want one matching the upstream knob, add a request.

Note: There is also a cap_mini part which covers less of the PCB and can be mounted after the knob assembly, if someone prefers it.

Printing tips:

* This part would also look better if printed lying on its side, but I haven't been successful with it, since it easily moves a little. But for this part it looks quite ok also if printed lying down.
* If you have fitted the reset switch, you must manually complete the matching square hole (there are two to allow for part mirroring)
* For right-hand mouse: Mirror about Y-axis

### bottom lid 
 ![](bottom.png?raw=true)

An optional part, only needed if you want to fill the bottom compartment with something to increase the weight.
Must be fastened with four M3 screws

Printing tips:

* For right-hand mouse: Same part

### foam_stencil
![](foam_stensil.png?raw=true)

This is a flattened and slightly shrunk version of the foam insert. 

Print it and use as a cutting stencil on 2 mm foam, leather, cork or other soft material.

Note: The holes were added just to save material and print time.

Printing tips:

* For right-hand mouse: Same part

### custom_target
![](custom_target_mod.png?raw=true)

This is a paper stencil for the "target" copper pieces.  Originally designed by https://github.com/lpurdy01/os3m_target_testing, but cut-off a bit to make assembly easier. There is also a pdf of the un-cut version, if you prefer. Both match the knob included here.

![](custom_target.png?raw=true)

Print the PDF on paper and use as stencil to cut copper sheet metal (1 mm thickness is fine). 

Printing tips:

* For right-hand mouse: Same part

## Assembly order and notes

Assuming you already have an assembled PBA and has removed all printing supports.

1. Make threads in the holes, at least a mm longer than you will need. Especially important in the stem and knob!  Ideally use an M3 taper, but an M3 screw will also do.
2. Glue copper pieces to the knob
3. Solder, if you want, wires to four switches and put them in place. Add the "button" parts.
4. Solder, if you want, a switch to the RX+TX holes or RX+3v3 holes on the bottom side. (Can be used to get the MCU into boot loader). 
  * There are a couple of push-holes prepared, depending of if you have two centered legs or two at one side. (And then two more for the case that you have mirrored the base)
  * Use a sharp object to push through the bottom in the hole best matching your switch
  * If you don't add the switch you probably want to drill the base hole bigger to be able to shorten the Rx and Tx with a piece of wire or similar (Not ESD safe). You could of course also sacrifice one of the buttons for this function.
5. Solder the button switch wires to the PCB (see below)
6. Screw PCB and Base together
7. Screw Stem and Flexure together
8. Screw Flexure (+Stem) and Knob together
9. Add the Cap to the Base (no screws)
10. Screw Stem and Base together
11. Add, if wanted, metall to the bottom compartment and fasten the lid.  (This step can be done at any time)

## Adding button switches

The button switches shall be 6x6x5mm, no bracket, either through-hole or SMT. 

Cut off the legs on one side and solder wires on the other.

Make sure you remove all printing supports on the base.

Route the wires, place the switches and attach the "button" parts. 

![](3_switches_mounted.png?raw=true)

(To be continued)
