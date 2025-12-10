# Unit Tests

## TODO: Create unit tests for firmware modules

### Test Framework
- [ ] Set up Unity test framework or similar
- [ ] Configure test build system
- [ ] Set up automated test execution

### Tests to Create

#### ADC Module Tests (`test_adc.c`)
- [ ] Test ADC initialization
- [ ] Test single channel read
- [ ] Test multi-channel scan
- [ ] Test voltage conversion accuracy
- [ ] Test filtering algorithms

#### SoC Estimation Tests (`test_soc_estimation.c`)
- [ ] Test Coulomb counting
- [ ] Test voltage-based estimation
- [ ] Test SoC fusion algorithm
- [ ] Test edge cases (0%, 100%)
- [ ] Test temperature compensation

#### Temperature Monitor Tests (`test_temp_monitor.c`)
- [ ] Test NTC conversion
- [ ] Test multi-sensor reading
- [ ] Test averaging
- [ ] Test threshold detection

#### Safety Module Tests (`test_safety.c`)
- [ ] Test overvoltage detection
- [ ] Test undervoltage detection
- [ ] Test overcurrent detection
- [ ] Test overtemperature detection
- [ ] Test MOSFET control
- [ ] Test fault logging

#### Communication Tests (`test_comm.c`)
- [ ] Test packet parsing
- [ ] Test checksum calculation
- [ ] Test command handling
- [ ] Test data serialization

## Running Tests
```bash
# TODO: Add commands to run tests
cd tests/unit_tests
make test
```
