# LiteSound
This card provides stereo audio capability for the Apple IIGS computers.

This project was done in <b>KiCad 6.0.6</b> and may not work with older versions.

Installation and use manual is a Google Docs file and can be found at this URL:
https://tinyurl.com/39kpvvwv

The J25 header on the IIGS motherboard provides an analog audio signal, and address lines
to drive a demultiplexer which splits audio into Left & Right audio channels.

I'm using a [74HC4052D](https://www.digikey.com/en/products/detail/toshiba-semiconductor-and-storage/74HC4052D/6109174) demultiplexer
and a [TL074CDR](https://www.digikey.com/en/products/detail/texas-instruments/TL074CDR/276926) quad audio op-amp.  There are other pin-compatible
chips that can be substituted.

Current(ish) board rendering:
[PCB rendering](IIGS-audio.png)

<b>Known issue:</b> This stereo sound card makes a chirp / squawk sound when the IIGS is switched off if a Reactive Mircro power supply is installed.   This does not happen
if your system uses an original power supply and does not impact performance in any way.  It may do the same with other aftermarket power supplies. YMMV.
