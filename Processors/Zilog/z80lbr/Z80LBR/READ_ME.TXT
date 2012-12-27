Perhaps you will want to make changes to parts of the source files.
All components are included for practical purpose, or as an
educational exercise.

Since an EAGLE script file cannot call another script file, it will
take a few minutes of your time to rebuild the library.  However,
it is very simple.  Execute the scripts in the following order, and
you should have no problem:


SCRIPT NCX@.SCR;          (provides NC "no connect" pins)
SCRIPT PWR@.SCR;          (provides VCC/GND component)
SCRIPT SMD@.SCR;          (supplies PLCC-44, QFP-44 packages)
SCRIPT PLC@.SCR;          (supplies PLCC Socket package)
SCRIPT DIP@.SCR;          (supplies DIP-40, DIP-28 packages)
WRITE;          (to save the file)
SCRIPT CPU\CPU-SYM.SCR;   (symbol for Z80 CPU)
SCRIPT CPU\Z80CPU-P.SCR;  (CPU, DIP-40 device)
SCRIPT CPU\Z80CPU-V.SCR;  (CPU, PLCC-44 SMD device)
SCRIPT CPU\Z80CPU-S.SCR;  (CPU, PLCC-44 Socket)
SCRIPT CPU\Z80CPU-F.SCR;  (CPU, QFP-44 SMD device)
WRITE;          (to save the file)
SCRIPT CTC\CTC-SYM.SCR;   (symbol for Z80 CTC)
SCRIPT CTC\Z80CTC-P.SCR;  (CTC, DIP-40 device)
SCRIPT CTC\Z80CTC-V.SCR;  (CTC, PLCC-44 SMD device)
SCRIPT CTC\Z80CTC-S.SCR;  (CTC, PLCC-44 Socket device)
SCRIPT CTC\Z80CTC-F.SCR;  (CTC, QFP-44 SMD device)
WRITE;          (to save the file)
SCRIPT DMA\DMA-SYM.SCR;   (symbol for Z80 DMA)
SCRIPT DMA\DMA-SYMV.SCR;  (symbol for CMOS PLCC DMA with RESET)
SCRIPT DMA\Z80DMA-P.SCR;  (DMA, DIP-40 device)
SCRIPT DMA\Z80DMA-V.SCR;  (CMOS DMA, PLCC-44 SMD device)
SCRIPT DMA\Z80DMA-S.SCR;  (CMOS DMA, PLCC-44 Socket device)
SCRIPT DMA\Z80DMANV.SCR;  (NMOS DMA, PLCC-44 SMD device)
SCRIPT DMA\Z80DMANS.SCR;  (NMOS DMA, PLCC-44 Socket device)
WRITE;          (to save the file)
SCRIPT PIO\PIO-SYM.SCR;   (symbol for Z80 PIO)
SCRIPT PIO\Z80PIO-P.SCR;  (PIO, DIP-40 device)
SCRIPT PIO\Z80PIO-V.SCR;  (PIO, PLCC-44 SMD device)
SCRIPT PIO\Z80PIO-S.SCR;  (PIO, PLCC-44 Socket device)
SCRIPT PIO\Z80PIO-F.SCR;  (PIO, QFP-44 SMD device)
WRITE;          (to save the file)
SCRIPT SIO\SIO-SYM.SCR;   (symbols for all Z80 SIO variations)
SCRIPT SIO\Z80SIO-0.SCR;  (SIO/0, DIP-40 device)
SCRIPT SIO\Z80SIO-1.SCR;  (SIO/1, DIP-40 device)
SCRIPT SIO\Z80SIO-2.SCR;  (SIO/2, DIP-40 device)
SCRIPT SIO\Z80SIO-3.SCR   (SIO/3, QFP-44 SMD device)
SCRIPT SIO\Z80SIO-4.SCR   (SIO/4, PLCC-44 SMD device)
SCRIPT SIO\Z80SIO4S.SCR   (SIO/4, PLCC-44 Socket device)
WRITE;          (to save the finished library)

26 OCT 1999
<beattidp@ieee.org>
