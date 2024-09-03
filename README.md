# LiteSound
This card provides stereo audio capability for the Apple IIGS computers.

This project was done in <b>KiCad 6.0.10</b> and may not work with older versions.

Installation and use manual is a Google Docs file and can be found at this URL:
https://tinyurl.com/39kpvvwv

The J25 header on the IIGS motherboard provides an analog audio signal, and address lines
to drive a demultiplexer which splits audio into Left & Right audio channels.

You can find partially made cables on eBay by searching for 7 pin 2510 or KF2510 cables, 30cm long.  
This length is "about right" and will reach all slots.  Pin 1 on the J25 goes to pin 7 on the LiteSound board.  
This is basically flipped or wired backwards.  Yeah, I should've caught this and may someday fix it.  
It's easy enough to just wire this way!   Included is a closeup photo of both ends of the cable, one end
attached to the PCB, and the other with the alignment tabs for the J25 end clearly visible.

The pins I use are [Molex 16-02-0103](https://www.mouser.com/ProductDetail/538-16-02-0103) on the LightSound end,
and the housings are [Molex 50-57-9207](https://www.mouser.com/ProductDetail/538-50-57-9207).

I'm using a [74HC4052D](https://www.digikey.com/en/products/detail/toshiba-semiconductor-and-storage/74HC4052D/6109174) demultiplexer
and a [TL074CDR](https://www.digikey.com/en/products/detail/texas-instruments/TL074CDR/276926) quad audio op-amp.  There are other pin-compatible
chips that can be substituted.

The headphone jack I use is a [CUI Devices SJ1-3515N](https://www.mouser.com/ProductDetail/490-SJ1-3515N) and the
7 pin header is an [Amphenol 77315-124-07LF](https://www.mouser.com/ProductDetail/649-77315-124-07LF).

Current(ish) board rendering:
[PCB rendering](IIGS-audio.png)

<b>Known issue:</b> This stereo sound card makes a chirp / squawk sound when the IIGS is switched off if a Reactive Mircro power supply is installed.   This does not happen
if your system uses an original power supply and does not impact performance in any way.  It may do the same with other aftermarket power supplies. YMMV.
