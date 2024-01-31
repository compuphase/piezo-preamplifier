# Piezo Pickup Preamplifier
These are simple designs for high impedance preamplifiers. They are intended for
piezo pickups, and in particular for piezo bridge pickups for (nylon-stringed)
guitars. There is a single-channel and a dual-channel design.

The designs are in KiCad. PDFs with the schematics, and the Gerber files for the
PCBs are also provided.

## Single channel
This circuit was built for use with a Shadow SH097 bridge pickup. The pickup has
a capacitance of 680pF. Yet, input impedance of this preamplifier is *only*
1M&Omega;, because the basses were already quite pronounced.

It is a pretty classic opamp circuit. Amplification is fixed at 1&times;
&mdash;the circuit is only to adapt the impedance (piezo bridge pickups are
pretty loud already). The main feature of the circuit is that it is compact,
and especially narrow. The idea is to fit this preamplifier into a slot
immediately below the pickup.

The PDF with the schematic also shows the wiring for a TRS socket and battery;
these are not on the PCB, and technically not part of the circuit). The main
idea of the wiring is that the battery is connected only when the jack plug is
inserted. When the plug is pulled out of the instrument, the battery is disconnected.

## Dual channel
This circuit was built for the ARTEC PG-333 bridge pickup. The pickup connects two
piezo bridge pickups in parallel, where each pickup covers only three strings. For
use with this preamplifier, the two piezo segments have to be separated, and each
connected to a separate input of the preamplifer.

I measured one of the piezo segments to have a capacitance of 580pF and the other
as 970pF &mdash;to my surprise. This being the case, you will want to position
the 580pF segment at the treble side, and the 970pF segment at the bass side of
the bridge.

The dual-channel circuit has two independent impedance converters, and a third
preamplifier to mix the outputs of the first stages. The gain of the "treble"
stage can be adjusted relative to the "bass" gain, with a trimmer pot.

---

Copyright 2023-2024, CompuPhase, Thiadmer Riemersma<br>
This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (https://creativecommons.org/licenses/by-nc-sa/4.0/).

