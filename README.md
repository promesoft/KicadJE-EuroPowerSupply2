# KicadJE-EuroPowerSupply2
4HP PSU faceplate with 80x100mm PSU + PDU board. Faceplate input from a laptop PSU (19V) and may be daisychained to the next Eurorack unit.

# Vital Components

# Status - mounted in rack
## Initial 
| Stage  | Detail | Status |
| ------------- | ------------- | ------------- |
| create material  | sch | done |
| | pcb |  done |
| | gerber | done |
| production  |   | done |
|  | produced | done |
|  | delivered | done |
## Preliminary validation
| Test  | Detail | Status |
| ------------- | ------------- | ------------- |
| Initial Inspection | | good alignment w panel - panel: pwr holes 2 mm too small |
| Initial Technical Test |  | OL LED's lighting up without load |
| Initial Technical Test |  | OL LED's ok with 2k2 but unsure of how they work now - 3k9 is ok without load but makes a bit of a light at a few 100 mA |
| Initial Technical Test |  | input fuse experienced a few problems after shoring the input of the DC-DC by mistake
| Initial Product Test |  | ok - Powers the uP DAC nicely|

## Secondary validation
| Test  | Detail | Status |
| ------------- | ------------- |------------- |
| Product Test |  | |
| Product Test |  | |
| Quality |  | |
| Quality | | |
| Long Term Product Test |  |  |
| Power Draw |  | 

## Errata
### Errata - 
Holes for Pwr in and out are 2mm too small in face plate

## Issues and Notes
There is just enough room on the front PCB to add a JST header for power feed to baseboard.

Input cap = 470uF/50V

Reg input cap 470uF/16V for 5V

Reg input cap 100uF/35V for +-12V

Reg output cap 470uF/16V for all

Only half the headers has decoupling caps

Not easy to measure the OL circuit as it is VERY close to the DC-DC input

Add current limiter on input and consider changing from OL to currentlimier with limit indication

Consider calc initial regulator stage as Capacitor multiplier and add small signal BJT in darlington config.
 - https://www.google.com/search?q=eeblog+david+jones+capacitor+multiplier&oq=eeblog+david+jones+capacitor+mul&aqs=chrome.1.69i57j33.18679j1j7&sourceid=chrome&ie=UTF-8

Place +/-15v header away from heatsink area.

# Pictures
![](KicadJE-EuroPowerSupply2_top.png)
![](KicadJE-EuroPowerSupply2_bottom.png)
# Schematic

## Prototype


# Inspiration
## Rev 1
https://github.com/promesoft/KicadJE-EuroPowerSupply
