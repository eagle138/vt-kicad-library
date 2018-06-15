# vt-kicad-library

Custom KiCad parts library containing parts not available in KiCad's default kicad-library repository or Digi-Key's digikey-kicad-library. This repository attempts to follow Digi-Key's organizational structure for ease of component purchasing.

## Creating a Custom Component

If a component schematic symbol or footprint required for a board is not already available in KiCad's default kicad-library repository, Digi-Key's digikey-kicad-library repository, or this repository, then a new component symbol or footprint must be created. The following guidelines should be followed for schematic symbol and footprint creation:

### Schematic Symbols:

Schematic symbols, specifically ICs, should follow these appearance guidelines.

- (A) Pin length:
- (B) Pin name size:
- (C) Pin number size:
- (D) Separation between pins:
- (E) Separation between pin and
- (F) Fill component background

Avoid multi-part components unless doing do greatly improves organization. Pins do not necessarily need to be placed in order; if moving a pin allows wires to be uncrossed or placed in a more organized way then moving the pin is preferred.

Add documentation to the component by going to `Edit component properties -> Description`. Under `Description`, paste the part's description from Digi-Key or a short description of the part. Under `Keywords`, place the part's Digi-Key part number, or manufacturer part number. Under `Documentation File Name`, place a link to the part's datasheet.

To save a new schematic symbol, first determine the [family](http://www.eewiki.net/display/Resources/Become+a+Digi-Key+Master#BecomeaDigi-KeyMaster-Digi-KeyTerminology) that the component belongs to in Digi-Key. If the part is not on Digi-Key, make your best guess based on the part's function. If the part's family already has a library (.lib) file in this repository, save the component to that library. If the family library file does not exist, save it to a new library file in the `vt-symbols` folder using the following naming scheme:

`vt_Family-Name.lib`

### Footprints

Follow the part's datasheet's recommended footprint layout.  
