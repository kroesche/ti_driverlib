TI Stellaris/Tiva Driverlib
---------------------------

This is the TI driver library for Stellaris/Tiva microcontrollers
(LM3S/LM4F/TM4C).  This is part of the software package known as
StellarisWare, or TivaWare, or SW-TM4C-something. This repo is only
the `driverlib` component which has a BSD-style license.  The rest of
the *Ware package is under a proprietary license so I did not include
it here. There is also a `third_party` directory that has third party
software under various licenses, also not included here. If you need
any of those other pieces you need to get it from TI.

The `inc` directory contained definitions for every part. This directory
alone is over 100 MB and has over 300 header files. Because of this I
removed all the part definition header files and I just add the specific
one I need to my project repo.

I use this repo as a submodule of my MCU projects that need to use the
driverlib. It has snapshots of driverlib releases over time. The commits
are tagged with the name of the release.  The following table shows the
tags so you can checkout a specific tag if you need a specific release.

Tag | Comment
----|--------
LM3S-LM4F-9453|This was the last release of StellarisWare that included both the LM3S and LM4F devices before the Tiva rebranding
LM3S-10636    |Last release of StellarisWare for just the LM3S device. After this the LM4F/Tiva devices were split into a separate product. This is probably what you should use if you have a LM3S.
TivaWare_C_2.0.1.11577|Likely the first, or nearly the first release of TivaWare after Tiva was split from Stellaris. Use this or a later release if you have Tiva (LM4F or TM4C)

* * * * *

_All Texas Instruments (TI) trademarks referenced here are the property
of Texas Instruments and the reference does not indicate any relationship
or endorsement by TI of the owner of this repository._

