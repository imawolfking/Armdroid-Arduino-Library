**************************************************
* PLEASE NOTE - THIS LIBRARY IS WORK IN PROGRESS *
**************************************************


This is the Armdroid Library for Arduino & Arduino wiring compatible micro-controllers.

Currently, the library has only been tested with the Arduino Leonardo, other boards
however may work without modification.  If you discover a problem with compilation, or
execution, then please let me know and I may decide to support your board in a
forthcoming release.

The SerialDriver example sketch is included with this library.   This is a complete,
ready to use embedded Armdroid driver program that responds to commands sent by USB/Serial
and manipulates the joints.

If, like me, your using the Arduino Leonardo board and intend communicating using hardware
serial pins (RX pin 0 and TX pin 1) instead of USB/Serial you will need find & replace all
occurrences of "Serial" and change to "Serial1" before compiling & uploading the Sketch.


More example programs & circuits coming soon!  Do check http://armdroid1.blogspot.co.uk
regularly for latest news, updates, and projects centered around this Arduino library.


Written by Richard Morris
Refer to the included LICENSE for licensing information


INSTALLATION

To download. Click the DOWNLOADS button in the top right corner, rename the uncompressed
folder Armdroid

Place the Armdroid library folder in your <arduinosketchfolder>/libraries/ folder.  You
may need to create the libraries subfolder if its your first library.  Restart the IDE


TROUBLESHOOTING

Stepper motors not running smoothly, or momentarily change direction
- try removing IC5 (74LS366) if installed, I am still investigating this issue.

Welcome message not shown when connecting an Arduino Uno
- i've had reports this message is not shown on startup, probably sometime to do with the
  changes in USB support and auto reset.  Serial driver should still function.
