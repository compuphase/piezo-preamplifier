# Piezo Pickup Preamplifier
This is a simple design for a high impedance preamplifier. It is intended for
piezo pickups, and in particular for piezo bridge pickups for (nylon-stringed)
guitars. Amplification is fixed at 1&times; &mdash;the circuit is only to adapt
the impedance (piezo bridge pickups are pretty loud already).

I used this circuit with a Shadow SH097 bridge pickup, which I measured to have 
a capacitance of 680pF. Yet, input impedance of this preamplifier is *only* 1M&Omega;, 
because the basses were already quite pronounced.

It is a pretty classic opamp circuit, with the main feature being that it is
quite compact (and notably: narrow). The idea is to fit this preamplifier into
a slot immediately below the pickup.

The design is in KiCad. A PDF with the schematic, and the Gerber files for the
PCB are also provided.

The circuit also shows the wiring for a TRS socket and battery; these are not on
the PCB, and technically not part of the circuit). The main idea of the wiring is
that the battery is connected only when the jack plug is inserted. When the plug
is pulled out of the instrument, the battery is disconnected.

Copyright 2023, CompuPhase, Thiadmer Riemersma<br>
This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0
 International License (https://creativecommons.org/licenses/by-nc-sa/4.0/).

