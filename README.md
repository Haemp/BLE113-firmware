BLE113-firmware
===============

BGScript API reference
---------------------

https://www.bluegiga.com/protectedstore/8pHYFByrRbCfvauWLt5CMQ/NotSzwA-2z-ynH1iG1tdIQ/U18PmIkDuWt-CmvSsN9B3ohK1z9PMvdyxfkmjDGPZMPTnXa4GMbm/Bluetooth_Smart_Software_v13_API_Reference.pdf

* Set function of port - Input or output - call hardware_io_port_config_function(port, function)(result)
* Setup pull up or down - call hardware_io_port_config_pull(port, tristate_mask, pull_up)(result)
* Set direction of port - rising or falling on edge - call hardware_io_port_irq_direction(port, falling_edge)(result)
* Activate port - call hardware_io_port_irq_enable(port, enable_bits)(result)
* Event handler for interupts - event hardware_io_port_status(timestamp, port, irq, state)
