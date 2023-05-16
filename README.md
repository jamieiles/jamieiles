I am a software engineer from the UK, working at
[Qualcomm](https://www.qualcomm.com/home) (and Nuvia pre-acquisition) where
amongst other things I'm responsible for pre-silicon software enablement
covering application processor firmware, operating systems and virtual
platforms on our custom CPU designs.

Prior to Nuvia/Qualcomm, I was the engineering team lead for
[Ksplice](http://ksplice.oracle.com/) at Oracle which provides rebootless OS
updates for Linux systems. I have a keen interest in CPU architecture and all
things low-level. I have designed three CPU's - a RISC-V RV32IMA core, a [x86
compatible](https://github.com/jamieiles/80x86) and another [home-grown 32-bit
RISC](https://github.com/jamieiles/oldland-cpu), all with SoC reference
designs.

My RV32IMA RISC-V core is implemented in SystemVerilog and offers ~2.61
CoreMark/MHz. The core implements the privileged architecture with SSTC and
Sscofpmf extensions and runs mainline Linux. I implemented a number unique
tracing techniques to record and replay execution to generate ELF core-files
for software debug. The core is a scalar design with parallel execution units
and out of order completion, register rename and dynamic branch prediction.
The system runs on a Spartan 7 FPGA and has been hardened with OpenLane for
the SKY130A process.

I have created an [80186](https://github.com/jamieiles/80x86) compatible IP
core from scratch which currently runs at 60MHz on a Cyclone V FPGA in ~1750
ALMs, implementing the full 80186 ISA, traps, faults + interrupts along with a
JTAG TAP. The core has a comprehensive test suite using Verilator + Google
Test, a C++ model to verify against, and a build system using CMake+Docker. A
reference design includes an SDRAM controller, MCGA graphics, PS/2
keyboard+mouse controller, fixed disk emulation on an SD card, lightweight
PIC+PIT implementations and a BIOS. The system can run a wide range of DOS
based applications with good performance.

See the rest of my projects on GitHub and more information on my [personal
website](https://www.jamieiles.com).
