## Hardware Schematics

This directory contains circuit schematics for the MicroGuard BMS.

### Files
- `main_schematic.kicad_sch` - Main circuit schematic
- `power_stage.kicad_sch` - Power management circuitry
- `cell_monitoring.kicad_sch` - Cell voltage monitoring circuit
- `protection.kicad_sch` - Protection circuitry
- `communication.kicad_sch` - Communication interfaces

### TODO
- [ ] Design main power supply circuit
- [ ] Design cell voltage measurement circuit (multiplexed ADC)
- [ ] Design current sensing circuit (shunt resistor + op-amp)
- [ ] Design temperature sensing circuit (NTC thermistors)
- [ ] Design protection MOSFETs circuit
- [ ] Design microcontroller section
- [ ] Design communication interfaces (I2C, UART, CAN)
