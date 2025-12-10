# API Reference

## Communication Protocol

### TODO: Document UART Protocol

#### Command Format
```
TODO: Define packet structure
- Start byte
- Command byte
- Length
- Data payload
- Checksum
```

#### Command Reference

##### CMD_GET_STATUS (0x01)
```
TODO: Document command
- Description
- Request format
- Response format
- Example
```

##### CMD_GET_VOLTAGE (0x02)
```
TODO: Document command
```

##### CMD_GET_CURRENT (0x03)
```
TODO: Document command
```

##### CMD_GET_SOC (0x04)
```
TODO: Document command
```

##### CMD_GET_TEMP (0x05)
```
TODO: Document command
```

##### CMD_SET_CONFIG (0x10)
```
TODO: Document command
```

##### CMD_CLEAR_FAULTS (0x11)
```
TODO: Document command
```

##### CMD_RESET (0x12)
```
TODO: Document command
```

### TODO: Document I2C Protocol

#### Register Map
```
TODO: Define register addresses
- 0x00: Device ID
- 0x01: Status register
- 0x02-0x03: Voltage MSB/LSB
- 0x04-0x05: Current MSB/LSB
- 0x06: SoC
- 0x07: Temperature
- 0x08: Fault flags
- etc.
```

#### Read/Write Operations
```
TODO: Document I2C read/write procedures
```

### TODO: Document CAN Protocol

#### Message IDs
```
TODO: Define CAN message IDs
- 0x100: Status message
- 0x101: Voltage data
- 0x102: Current data
- 0x103: Temperature data
- 0x104: Fault message
- etc.
```

#### Message Formats
```
TODO: Document CAN message structure for each ID
```

## Data Structures

### TODO: Document key data structures

#### Battery Status Structure
```c
// TODO: Define and document structure
```

#### Configuration Structure
```c
// TODO: Define and document structure
```

## Error Codes

### TODO: Document all error/fault codes
- 0x01: Overvoltage
- 0x02: Undervoltage
- 0x04: Overcurrent charge
- 0x08: Overcurrent discharge
- 0x10: Short circuit
- 0x20: Overtemperature
- etc.
