# passive-toolchanger
A concept for 3d printer toolchanger which uses only the existing X- and Y-movements to lock and unlock the toolhead

## What is passive-toolchanger?
This project was inspired by existing toolchangers. They all used additional hardware to lock and unlock the tool.
This is usually done by a motor that rotates a lock or by an electromagnet. \
I wanted to find a way to lock and unlock the toolhead with the allready existing stepper motors for the X- and Y-movement.

I am not sure if this has any benefit, but somehow it became a personal challenge.
All what I am publishing here is only "proof of concept" because I do not have a printer that can be transfered to a toolchanger yet.

## References
Starting point for this project were the tool_carrier and the tool_template from [jubilee](https://github.com/machineagency/jubilee) printer project by Joshua Vasquez of Machine Agency at the University of Washington.

## Variants
### Magnet wheel toolchanger
The [magnet-wheel-toolchanger](magnet-wheel-toolchanger) uses a wheel with magnets, that is rotated by a cograil. The cograil holds the wings that fit into the tool-post. When inside the tool-post, the cograil is fixed left/right and the wheel can be rotated by moving the tool-plate. 


### Magnet Slider Toolchanger


### Snap-In Toolchanger
(Inspired by my Espresso machine)


### mushroom striker Toolchanger

## Disclaimer
I develop with RS components DesignSpark mechanical which seems to be a stripped down version from spaceclaim. Unfortunatly, export to STEP is not possible in the free version.

Construction is not optimized to be perfect printable but for me, everything printed without support.

I do not have a 3D printer that is possible to be transfered to a toolchanger yet. 
All of the files are designed to work on my current printer Easythreed K1. This printer has geared stepper motors and thus has backlash on all three axis. The results will be different when printing on a printer without backlash.

### Who am I?
passive-toolchanger was designed by [Martin Voelz]

### Open Source
passive-toolchanger is licensed under a [Creative Commons Attribution 4.0 Unported License](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0)
