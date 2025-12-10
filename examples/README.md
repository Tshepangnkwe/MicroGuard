# Example Configurations

This directory contains example configuration files for different battery types and applications.

## TODO: Create example configurations

### `config_4s_lion_2500mah.h`
```c
// TODO: 4S Li-ion configuration for 2500mAh cells
// Example: 18650 cells in 4S configuration
```

### `config_3s_lipo_5000mah.h`
```c
// TODO: 3S LiPo configuration for 5000mAh pack
// Example: RC battery pack
```

### `config_6s_nimh_2000mah.h`
```c
// TODO: 6S NiMH configuration for 2000mAh cells
// Example: Power tool battery
```

### `config_8s_lifepo4.h`
```c
// TODO: 8S LiFePO4 configuration
// Example: Solar storage application
```

## Usage

1. Choose the configuration that matches your battery
2. Copy the configuration values to `firmware/inc/config.h`
3. Rebuild the firmware
4. Flash to the device

## Creating Custom Configurations

### TODO: Document configuration steps
- [ ] Determine battery chemistry
- [ ] Count number of cells in series
- [ ] Find cell datasheet
- [ ] Set voltage limits
- [ ] Set current limits
- [ ] Set temperature limits
- [ ] Calibrate measurements
