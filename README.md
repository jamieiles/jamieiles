I am a software engineer from the UK, leading the Operating Systems team for
the Nuvia SoCs at [Qualcomm](https://nuviainc.com/) (and Nuvia
pre-acquisition) where we're creating new SoCs with leading performance and
energy efficiency for the data center.

Prior to Nuvia/Qualcomm, I was the engineering team lead for
[Ksplice](http://ksplice.oracle.com/) at Oracle which provides rebootless OS
updates for Linux systems. I have a keen interest in CPU architecture and all
things low-level. I have designed three CPU's - a RISC-V RV32IMA core, a [x86
compatible](https://github.com/jamieiles/80x86) and another [home-grown 32-bit
RISC](https://github.com/jamieiles/oldland-cpu), all with SoC reference
designs.

I have created an [80186](https://github.com/jamieiles/80x86) compatible IP
core from scratch which currently runs at 60MHz on a Cyclone V FPGA in ~1750
ALMs, implementing the full 80186 ISA, traps, faults + interrupts along with a
JTAG TAP. The core has a comprehensive test suite using Verilator + Google
Test, a C++ model to verify against, and a build system using CMake+Docker. A
reference design includes an SDRAM controller, MCGA graphics, PS/2
keyboard+mouse controller, fixed disk emulation on an SD card, lightweight
PIC+PIT implementations and a BIOS. The system can run a wide range of DOS
based applications with good performance.

The [Oldland CPU](https://github.com/jamieiles/oldland-cpu) is my first
home-grown CPU, a full-featured 32-bit RISC CPU, written in Verilog and
synthesizable on Intel FPGAs. The CPU features a 5 stage pipeline, privilege
modes, caches, TLB's and a debug controller. The SoC has an SDRAM controller,
SPI master, UART, timers, interrupt controller and other peripherals.  I have
also ported binutils, gcc, newlib, u-boot and RTEMS to the Oldland
architecture.

See the rest of my projects on GitHub and more information on my [personal
website](https://www.jamieiles.com).
