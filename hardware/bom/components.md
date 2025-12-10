# Bill of Materials (BOM)

## TODO: Create BOM with the following components

### Microcontroller
- [ ] STM32 or similar ARM Cortex-M MCU (low power)
- [ ] Crystal oscillator
- [ ] Decoupling capacitors

### Power Supply
- [ ] LDO voltage regulator (3.3V)
- [ ] Input/output capacitors
- [ ] Protection diodes

### Cell Monitoring
- [ ] Multiplexer IC (for multi-cell voltage measurement)
- [ ] Precision voltage reference
- [ ] ADC (if not integrated in MCU)
- [ ] Input protection resistors

### Current Sensing
- [ ] Precision shunt resistor (low resistance, high power)
- [ ] Instrumentation amplifier or op-amp
- [ ] Filter capacitors

### Temperature Monitoring
- [ ] NTC thermistors (multiple)
- [ ] Pull-up resistors

### Protection
- [ ] N-channel MOSFETs (for charge/discharge control)
- [ ] Gate driver IC (optional)
- [ ] Fuse or PTC
- [ ] TVS diodes

### Communication
- [ ] CAN transceiver (optional)
- [ ] Level shifters (if needed)
- [ ] Connectors (JST, terminal blocks)

### Passive Components
- [ ] Resistors (various values)
- [ ] Capacitors (ceramic, electrolytic)
- [ ] Inductors (if needed for filtering)
- [ ] LEDs (status indicators)

### Connectors
- [ ] Battery connector
- [ ] Load connector
- [ ] Programming header (SWD/JTAG)
- [ ] Communication connectors
