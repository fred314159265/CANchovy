# CANchovy USB-CAN Interface

This repository contains the design file for an isolated USB-CAN interface PCB. It is based upon the MKS CANable V2.0 and is compatible with the [CANable V2.0 firmware](https://github.com/normaldotcom/canable2-fw). It connects to the CAN bus via RJ45 connectors which can be configured with whatever pinout you require!


<img src="Images\PCB-Top.png" alt="PCB-Top" style="zoom: 43%;" />

<img src="Images\PCB-Bottom.png" alt="PCB-Top" style="zoom: 45%;" />

## Features

* Firmware compatible with [CANable V2.0 firmware](https://github.com/normaldotcom/canable2-fw) - can be flashed & updated with the [CANable 2.0 web updater](https://canable.io/updater/canable2.html).
* RJ45 pinout configured via solder-able jumpers.
* Galvanic isolation between CAN port and USB.
* Two RJ45 connector in parallel allows for inserting inline on bus - all eight signal are passed through.
* DIP switch to enable or disable CAN termination.
* DIP switch to enable silent mode, preventing the CANchovy from transmitting on the bus in hardware.
* JLCPCB basic parts used where possible and all parts available for JLCPCB assembly service. Five CANchovies fully assembled with postage costs around $20 per CANchovy.
* 3D printed case design files.

# Status

Assembled CANchovies from JLCPCB of both revision A & B have been tested and work correctly. The only issues with these version were silkscreen issues.

Revision C has the silkscreen fixed and is ready to manufacture and use.

# Configuring RJ45 Connections

As mentioned above, a feature of this board is that the RJ45's pinout is user configurable. By soldering one jumper for each of the three connections (0V, CAN_H, CAN_L) on the rear of the board, your custom CAN pinout over RJ45 can be supported!

Simply bridge one of the solder jumpers in each of the silkscreen boxes (labelled: 0V, CAN_H & CAN_L) to connect each signal to the corresponding pin number of the RJ45 connectors.

__⚠⚠⚠ Care must be taken to ensure no two signals are connected to the same RJ45 pin! ⚠⚠⚠__

<img src="Images\PinMapping.png" alt="PCB-Top" style="zoom: 45%;" />
