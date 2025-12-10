# Firmware Libraries

## Third-Party Libraries

### CMSIS (Cortex Microcontroller Software Interface Standard)
- Core peripheral access
- DSP functions
- RTOS support

### Device HAL (Hardware Abstraction Layer)
- MCU-specific drivers
- STM32 HAL, Nordic SDK, or similar

### TensorFlow Lite for Microcontrollers
- Lightweight ML inference engine for pre-trained models
- Quantized model support
- ~50KB footprint

## TinyML Setup

### Installation

```bash
# Clone TensorFlow Lite Micro repo
git clone https://github.com/tensorflow/tflite-micro.git lib/tensorflow-lite-micro
```

### Integration

1. Add TFLite Micro sources to build system
2. Place pre-trained models in `ml/models/`
3. Include model headers (e.g., `#include "ml/models/health_model.h"`)
4. Initialize interpreter in firmware
5. Run inference periodically on battery data

### Memory Requirements

- Model storage: 20-30KB Flash
- Runtime RAM: 10-20KB
- Inference scratch: 5-10KB

## Directory Structure

```
lib/
├── CMSIS/
│   ├── Include/
│   └── Source/
├── Device/
│   ├── Include/
│   └── Source/
├── tensorflow-lite-micro/
│   ├── tensorflow/
│   └── signal/
└── README.md
```
