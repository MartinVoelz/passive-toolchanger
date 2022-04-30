# magnet wheel toolchanger

## References
Starting point for this project were the tool_carrier and the tool_template from [jubilee](https://github.com/machineagency/jubilee) printer project by Joshua Vasquez of Machine Agency at the University of Washington.

## Intention
The idea was to create a toolchanging mechnism that can be handled by x- and y- movement of the tool-carrier.
The approach in this variant is to have three magnets in the carrier that are alligned in the same 120° star as the dovels and balls.

In the toolcarrier is also a 120° star of three magnets on a wheel. When the magnets are alligned with the carrier, that magnets connect both parts.
When the wheel is rotated 60° or -60°, than there is no magnetic force between tool-carrier and tool-template.

The wheel is actuated by a cogwheel - cograil mechanism. When in docking position, the cograil-slider is fixed in left / right direction.
When the carrier moves to left or right, the tool will move and the magnet-wheel will turn.

The cograil slider also has two magnets that are alligned with one of the magnet-wheel magnets in parking postition left or right. This ensures, that
the tool will stay in this position when not used.

## Changes
### Carrier
* Removed everything that was used for original turning lock and endswitches because I wanted to have a carrier without any wire
(Of course the switches must be put to another position in real life)
* Changed geometry to three connection screws between carrier and carrier baseplate. The original 2 upper screws were alligned with the magnets in parking position.

### Tool template
* base geometry and 120° dovel - ball connection was kept
* added magnet-wheel mechanism

### parking post
* original jubilee

## measurements
### pull off force
I used magnets 10mm x 3mm which were specified to have a holding force of 2.3 kg each.
The distance between the carrier plate and the spinning wheel is less than 1mm.

Measurement to be done

### sliding force
To unlock the tool from the carrier, the wheel must be rotated left or right. This must be possible for the stepper motors without loosing steps.
The force that is needed for this can be adjusted by the size of the the cogwheel. Bigger cogwheel means less force but longer way to move

Measurement to be done

### way to move
In the current setup, the slider moves 9mm to the left or to the right to change between lock and park position.
This movement of the slider reduces the build area for the tool itself! In a real environtment, only one parking position is necessary.

## Disclaimer
I develop with RS components DesignSpark mechanical which seems to be a stripped down version from spaceclaim. Unfortunatly, export to STEP is not possible in the free version.

Construction is not optimized to be perfect printable but for me, everything printed without support.

I do not have a 3D printer that is possible to be transfered to a toolchanger yet. 
All of the files are designed to work on my current printer Easythreed K1. This printer has geared stepper motors and thus has backlash on all three axis. The results will be different when printing on a printer without backlash.

### Who am I?
passive-toolchanger was designed by [Martin Voelz]

### Open Source
passive-toolchanger is licensed under a [Creative Commons Attribution 4.0 Unported License](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0)
