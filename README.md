# DIY_BTSpeakerBox
This project presents a DIY design for a speaker box that can recieve audio data from an analog 3.5mm Jack or a BT module. It incorporates a 3-band Equalizer custom PCB that also functions as the main power distribution board.


The main components of the board are present in the HW wiring diagram attached; it consits of a main PCB that incorporates a PreAmp with 3 band EQ, a BT audio reciever module, and a 30W stereo class D amplifier. A 3D encasing is also provided (Step and FreeCAD project files are included in the Enclosure branch). A generic BT and Class D amp modules are used in this project; however, the main PCB is compatible with any alternative solution (either custom or commercial) that uses a similar voltage. Nontheless, note that the main PS (which is, effectively, directly connected to the amp) must be of at least 12V to ensure the proper operation of the 9V regulator.

This amplifier set up has been tested with a 12V 3A power supply over a low-medium volume range; over a 2 hour listening session no excessive heating was detected in either module of the product.

NOTE: A Mains to 12-24V power supply is not included in this design, it recieved power from a standard barrel adaptor using an external supply. It is highly recommeded to use a good quality supply to reduce noise in the PreAmp (This alternative has provided decent results during testing: https://a.co/d/3dhSiTF).

NOTE2: Rev 1.1 is the modified version of the main PCB with some mods from the Rev 1.0 already installed. this design is not tested; however, only minor changes were made so its functionallity is highly likely


Bellow is a list of the current known issues of the project:

-Main PCB is missing mounting wholes for easy attachment to the box (included in the newest revision but missing on the 3D desingn file).
-Noise floor of the PreAmp is noticeable at low volumes (TO DO: reduce all resistances by a factor of 10 and consider using non-carbon based resistors to reduce thermal noise)
-Missing Soft Start circuit to prevent Popping on Speakers during Power-Up/Down.
-Certain combinations of the bass/tremble/mid potentiometers generate an audible oscillation that is transmitted to the spakers; needs further investigation in the filter Op-Amp loop.


Feel free to adapt this project to your particular needs, all the design files are provided as Open Source. Furthermore, if a solution to any of the listed issues is found, a pull request with the approach would be highly appreciated.
