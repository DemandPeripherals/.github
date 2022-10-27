## The Peripheral Control Project

### What
 - Eliminate microcontrolers using an FPGA


### Why
- Lower development costs
    -  No uC firmware
    -  No need to learn FPGAs, Verilog, tool chains, or drivers
    -  Schematic is FPGA circuit + Pmods (could be automated)
- Lower BOM costs
    -  Just one FPGA with lots of IO and no real-time constraints
    -  Low end FPGA, ~4000 LUTs, no LVDS needed
    -  No need for FPGA flash, download from Linux at boot
- Off-the-Shelf
    - Off the shelf FPGA dev boards
    - Off the shelf Pmod modules (200+)
    - Off the shelf Wishbone peripheral per Pmod
    - Off the shelf Linux interface and protocol
    - Off the shelf Linux API with simple publish/subscribe
    - Off the shelf schematics
- Traditional Linux real-time control
    - microcontroller, often more than one
    - custom hardware required
    - custom uC software required
    - custom Linux interface required
    - custom Linux API required


### How
- Buy an FPGA dev card with Pmod connectors
- Select Pmod cards for your applicaiton
- Visit https://demandperipherals.com/build to select peripherals
    -  Portal backend software links all peripherals in FPGA image
    -  Receives FPGA binary in email
    -  Or build yourself from sources and a our Makefiles
- Install pcdaemon to get Linux API to peripherals
- Possible to get an "API complete" system in an hour
