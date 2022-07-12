# LiteSound
LiteSound stereo audio card for the Apple IIGS



This card provides stereo audio capability for the Apple IIGS computers.

The J25 header on the IIGS motherboard provides an analog audio signal, and decode lines
to drive a demultiplexer which splits audio into Left & Right audio channels.

I'm using a [74HC4052D](https://www.digikey.com/en/products/detail/toshiba-semiconductor-and-storage/74HC4052D/6109174) demultiplexer
and a [TL074CDR](https://www.digikey.com/en/products/detail/texas-instruments/TL074CDR/276926) quad audio op-amp.
