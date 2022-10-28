## What
- Eliminate microcontrolers using an FPGA

<br>

## Why
- Lower development costs
    -  No uC firmware
    -  No need to learn FPGAs, Verilog, tool chains, or drivers
    -  Schematic is FPGA circuit + Pmods (could be automated)
- Lower BOM costs
    -  Just one FPGA with lots of IO and no real-time constraints
    -  Low end FPGA, ~4000 LUTs, no LVDS needed
    -  No need for FPGA flash, download from Linux at boot
- Traditional Linux real-time control is expensive
    - microcontroller (often more than one)
    - custom hardware required
    - custom uC software required
    - custom Linux interface required
    - custom Linux API required
- Peripheral Control is Off-the-Shelf
    - Off the shelf FPGA dev boards
    - Off the shelf Pmod modules (200+)
    - Off the shelf Wishbone peripheral per Pmod
    - Off the shelf Linux interface and host protocol
    - Off the shelf Linux API with simple publish/subscribe
    - Off the shelf schematics

<br>

## How
- Buy an FPGA dev card with Pmod connectors
- Select Pmod cards for your applicaiton
- Visit https://demandperipherals.com/build to select peripherals
    -  Portal backend software links all peripherals in FPGA image
    -  Receives FPGA binary in email
    -  Or build yourself from sources and a our Makefiles
- Install pcdaemon to get Linux API to peripherals
- Possible to get an "API complete" system in an hour

<br>
<br>

<img src=https://raw.githubusercontent.com/PeripheralControl/.github/f227507d81ccfed5844605a8bbcf8907e0a3e2f5/profile/repoes.svg height=250 />
<br>
