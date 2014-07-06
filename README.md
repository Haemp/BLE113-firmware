Mr.Manhattan v0.3
=============

## Problems ##
- No easy way to program the external BLE-113.
- Programming the BLE-113 for multi input forwarding - theoretically solved.
- Creating a simplistic touch surface - theoretically solved.

## Todo ##
- Programming the BLE-113 to forward input from the test board buttons to the bluetooth dongle.
- Extend the existing manhattan app to read data from new low energy spec bluetooth config. 
- Solder extension cables to the fanstastically small bluetooth chip. 
- Transfer the firmware from the prototype board to the chip.
- Create binary input touch surface (start simple).
- Attatch chip on finger holster along with a serial connected cell battery and the touch surface.
- Celebrate 
- Go to bed
- Get up - go to work. Hey, what the hell do I know!

## BLE113-firmware resources ##
===============

BGScript API reference
---------------------
https://www.bluegiga.com/protectedstore/8pHYFByrRbCfvauWLt5CMQ/NotSzwA-2z-ynH1iG1tdIQ/U18PmIkDuWt-CmvSsN9B3ohK1z9PMvdyxfkmjDGPZMPTnXa4GMbm/Bluetooth_Smart_Software_v13_API_Reference.pdf

http://mt-system.ru/sites/default/files/documents/ble_application_note_crp_sensor.pdf

* Set function of port - Input or output - call hardware_io_port_config_function(port, function)(result)
* Setup pull up or down - call hardware_io_port_config_pull(port, tristate_mask, pull_up)(result)
* Set direction of port - rising or falling on edge - call hardware_io_port_irq_direction(port, falling_edge)(result)
* Activate port - call hardware_io_port_irq_enable(port, enable_bits)(result)
* Event handler for interupts - event hardware_io_port_status(timestamp, port, irq, state)
