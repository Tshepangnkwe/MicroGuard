# Calibration Tools

## ADC Calibration

### TODO: Create ADC calibration utility
- [ ] Python/C tool to measure and correct ADC offsets
- [ ] Procedure to measure known reference voltages
- [ ] Generate calibration coefficients
- [ ] Store calibration data in firmware

### Usage
```bash
# TODO: Add calibration tool usage
python adc_calibration.py --port COM3 --reference 3.300
```

## Current Sensor Calibration

### TODO: Create current sensor calibration utility
- [ ] Measure shunt resistor actual value
- [ ] Measure op-amp gain
- [ ] Calculate calibration factors
- [ ] Test with known load currents

## Temperature Sensor Calibration

### TODO: Create temperature calibration utility
- [ ] Measure NTC resistance vs temperature
- [ ] Fit Steinhart-Hart coefficients
- [ ] Verify against known temperatures

## SOC Calibration

### TODO: Create SoC calibration procedure
- [ ] Full discharge test to measure actual capacity
- [ ] Voltage-SoC curve measurement
- [ ] Update lookup tables

## Files
```
calibration/
├── adc_calibration.py       # TODO: Create this
├── current_calibration.py   # TODO: Create this
├── temp_calibration.py      # TODO: Create this
├── soc_calibration.py       # TODO: Create this
└── README.md
```
