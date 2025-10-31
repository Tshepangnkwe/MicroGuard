# Microguard

A low-power Battery Management System (BMS) built from scratch for portable electronics, IoT devices, and small-scale energy storage applications.

## Overview

Microguard is a comprehensive BMS solution designed to monitor and manage battery performance, health, and safety in low-power applications. The system ensures optimal battery operation, extends battery life, and provides robust safety features.

## Features

- **Cell Voltage Monitoring**: Precise measurement of individual cell voltages
- **State-of-Charge (SoC) Estimation**: Accurate battery capacity tracking using advanced algorithms
- **Temperature Monitoring**: Real-time thermal monitoring for safety
- **Safety Protection**: Overcharge, over-discharge, short circuit, and thermal runaway protection
- **Communication Interface**: I2C, UART, and CAN bus support for external integration
- **Low Power Design**: Optimized for minimal current consumption in standby mode

## Hardware

- Custom PCB design with modular architecture
- Support for Li-ion, LiPo, and NiMH battery chemistries
- Configurable for 2S to 8S battery packs
- Onboard voltage and current sensing with high precision ADCs

## Software

- Firmware written in embedded C
- Real-time monitoring and control algorithms
- Configurable parameters for different battery types
- Data logging and diagnostic capabilities

## Project Structure
```
microguard/
├── hardware/
│   ├── schematics/          # Circuit schematics
│   ├── pcb/                 # PCB design files (KiCad)
│   ├── bom/                 # Bill of Materials
│   └── datasheets/          # Component datasheets
├── firmware/
│   ├── src/                 # Source code
│   │   ├── main.c
│   │   ├── adc.c
│   │   ├── soc_estimation.c
│   │   ├── temp_monitor.c
│   │   ├── safety.c
│   │   └── comm.c
│   ├── inc/                 # Header files
│   ├── lib/                 # Libraries
│   └── build/               # Build output
├── simulation/
│   ├── spice/               # SPICE simulations
│   └── models/              # Battery models
├── docs/
│   ├── design_notes.md      # Design documentation
│   ├── user_manual.md       # User guide
│   ├── api_reference.md     # API documentation
│   └── safety_standards.md  # Safety compliance info
├── tests/
│   ├── unit_tests/          # Unit tests
│   └── integration_tests/   # Integration tests
├── tools/
│   └── calibration/         # Calibration utilities
├── examples/                # Example configurations
├── LICENSE
└── README.md
```

## Getting Started

### Prerequisites

- KiCad 7.0+ for PCB design
- GCC ARM toolchain or RISC-V toolchain (depending on MCU choice)
- Programming hardware (ST-Link, J-Link, etc.)
- Multimeter and oscilloscope for testing

### Building the Firmware
```bash
cd firmware
make clean
make all
make flash
```

### PCB Fabrication

1. Open the KiCad project in `hardware/pcb/`
2. Generate Gerber files
3. Submit to your preferred PCB manufacturer

## Configuration

Edit `firmware/inc/config.h` to configure:
- Number of cells in series
- Battery chemistry type
- Current sensing parameters
- Communication protocol settings

## Safety Warning

⚠️ **Warning**: Working with batteries can be dangerous. Always follow proper safety procedures, including:
- Never short circuit battery terminals
- Use proper fusing and protection
- Test in a controlled environment
- Follow local regulations for battery handling

## Roadmap

- [ ] Initial hardware design
- [ ] Firmware v1.0 with basic monitoring
- [ ] SoC estimation algorithm implementation
- [ ] Cell balancing circuitry
- [ ] Mobile app for monitoring
- [ ] Support for additional battery chemistries

## Contributing

Contributions are welcome! Please read the contributing guidelines before submitting pull requests.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
