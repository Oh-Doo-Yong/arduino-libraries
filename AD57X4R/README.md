AD57X4R
=======

Authors:

    Peter Polidoro <polidorop@janelia.hhmi.org>

License:

    BSD

Provides an SPI based interface to the AD57X4R Complete, Quad,
12-/14-/16-Bit, Serial Input, Unipolar/Bipolar Voltage Output DACs.

[Usage Examples](./examples)


##Wiring

    GND----| AVss          AVdd |--Vdd
    X------| NC           VoutC |--VoutC
    VoutA--| VoutA        VoutD |--VoutD
    VoutB--| VoutB     SIG\_GND |--GND
    GND----| BIN2SCOMP SIG\_GND |--GND
    X------| NC        DAC\_GND |--GND
    CS-----| ~SYNC     DAC\_GND |--GND
    SCK----| SCLK           REF |--||(1uF)--GND
    MOSI---| SDIN           SD0 |--MISO
    GND----| ~LDAC          GND |--GND
    +5V----| ~CLR          DVcc |--+5V
    X------| NC              NC |--X

    Vdd--||(10uF)--GND

    Vdd--||(0.1uF)--GND

    +5V--||(10uF)--GND

    +5V--||(0.1uF)--GND
