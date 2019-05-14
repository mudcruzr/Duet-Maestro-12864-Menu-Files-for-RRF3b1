# Duet-Maestro-12864-Menu-Files
A set of files to allow a Duet Maestro to present a basic menu system on a 12864 reprap graphic display.

Notes:

1. These menu files are for RepRapFirmware 3 beta 1 ONLY! Do not try to use them on any earlier version of RRF. I have no idea what would happen.
2. If you have a BLTouch probe and it's connected correctly to the zprobe connector on the Maestro, you must change your M558 line in config.g to include C"zprobe.in" and you must add a new M950 line to config.g

e.g. My M558 line is now: M558 P9 C"zprobe.in" H5 F300 T4000 A10 S0.003 R0.5 B1

and the last line in my config.g is: M950 S0 C"zprobe.mod"

Installation:

Download the complete set of files, unzip them and, using the DWC Display page, upload them to your /menu folder.

Beware, any existing files with the same name will be overwritten, so best backup first.
