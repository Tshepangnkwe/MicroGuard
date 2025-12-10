# TinyML for MicroGuard BMS

## Overview

TinyML integration for on-device inference using **pre-trained models** to predict battery health and detect anomalies.

## Pre-trained Models

This project uses pre-trained TensorFlow Lite models. Place your `.tflite` and `.h` model files in the `models/` directory.

### Model Sources

- Edge Impulse (pre-built battery monitoring models)
- TensorFlow Lite Model Zoo
- Research publications
- Battery monitoring datasets with pre-trained models

## Deployment Workflow

1. **Obtain pre-trained model** (`.tflite` format)
2. **Convert to C header** using `xxd` or TensorFlow tools
3. **Place in** `ml/models/` directory
4. **Include in firmware** build
5. **Initialize TFLite Micro** runtime in firmware
6. **Run inference** on battery data

## Firmware Integration

```c
// Include the model
#include "ml/models/health_model.h"

// Initialize TensorFlow Lite Micro
// Set up interpreter with model
// Run inference periodically
// Get predictions
```

## Model Requirements

- Format: TensorFlow Lite (`.tflite`)
- Quantization: INT8 preferred for efficiency
- Size: <30KB to fit in flash memory
- Inference time: <100ms target
- Input: Voltage, current, temperature, SoC
- Output: Health score or anomaly probability

## Directory Structure

```
ml/
├── models/              # Pre-trained model files
│   ├── health_model.tflite
│   ├── health_model.h
│   ├── anomaly_model.tflite
│   └── anomaly_model.h
└── README.md
```

## Performance Expectations

- **Memory**: 20-50KB (model + runtime)
- **Latency**: <100ms per inference
- **Power**: ~1-2mA during inference
- **Accuracy**: Depends on pre-trained model quality
