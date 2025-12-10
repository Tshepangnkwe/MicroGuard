# Pre-trained TinyML Models

## Model Files

Place pre-trained TensorFlow Lite models here:

- `health_model.tflite` - Battery health prediction model
- `health_model.h` - C header with model array (generated from .tflite)
- `anomaly_model.tflite` - Anomaly detection model  
- `anomaly_model.h` - C header with model array (generated from .tflite)

## Model Sources

You can obtain pre-trained models from:
- Research papers and publications
- Battery dataset repositories
- Edge Impulse Studio (pre-built models)
- TensorFlow Lite Model Maker
- Community repositories

## Converting TFLite to C Header

```bash
# Using xxd
xxd -i health_model.tflite > health_model.h

# Or using TensorFlow tools
python -m tensorflow.lite.python.util.convert_to_c_source health_model.tflite > health_model.h
```

## Model Specifications

Expected model characteristics:
- Input features: voltage, current, temperature, SoC, cycles
- Output: health score or anomaly probability
- Quantization: INT8 preferred
- Size: <30KB
- Inference: <100ms on ARM Cortex-M
