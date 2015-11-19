# gluino
bringing the main gluion features to the Arduino world

The top two reasons people bought the gluion sensor interface were OSC and its 16-bit converters.
These days (2015) there are a number of options to add Ethernet to the Arduino, but still no dedicated shields with better quality converters.

The gluino therefore will combine these two features onto a single shield.

If possible I will try to add headers for a Teensy, as that's the interface I use the most these days.

One problem will be to share the SPI between the Ethernet chip (probably WIZ5100) and the ADS8344 converters. I can't really use a different ADC as I have way too many of them in stock. But as I don't want to rewrite the existing Ethernet libraries I'd also prefer to stay with an existing solution. 
So I'll have to figure out wether SPI could be shared in a way that would allow for acceptable update rates.
