# Infineon ML Middleware Support for Zephyr

## Overview
This package provides the Zephyr integration layer for Infineon Machine Learning Middleware in the HAL downstream workspace. It enables TensorFlow Lite Micro based inference through the `mtb_ml_*` API set and adds Zephyr-specific build, configuration, and compatibility glue for supported Infineon targets.

## Features
The package includes:
* Zephyr module integration files (`module.yml`, `Kconfig`, `CMakeLists.txt`) for seamless enablement in Zephyr applications
* `mtb_ml_*` API compatibility support so existing ML Middleware application code can be reused with Zephyr
* Inference engine selection for TensorFlow Lite Micro with either interpreter or interpreter-less operation
* Quantization options for `float32`, `int8`, and `int16` model execution
* Optional hardware acceleration paths:
	* Infineon NNLite NPU support for Cortex-M33 targets
	* ARM Ethos-U55 NPU support via ML Middleware for Cortex-M55 targets
* Optional Zephyr-native TensorFlow backend selection while preserving ML Middleware APIs
* Configurable runtime settings for tensor arena size, model count, auto initialization, cache management, and log level
* Optional data streaming and performance monitoring support for model validation and profiling

## More information
Use the following links for more information, as needed:
* [Zephyr integration sources](./zephyr)
* [TensorFlow Lite Micro package](../ml-tflite-micro/README.md)
* [ModusToolbox(TM) Machine Learning Design Support](https://www.infineon.com/cms/en/design-support/tools/sdk/modustoolbox-software/modustoolbox-machine-learning/)
* [Infineon GitHub](https://github.com/infineon)
* [ModusToolbox(TM)](https://www.infineon.com/design-resources/development-tools/sdk/modustoolbox-software)

© 2026, Cypress Semiconductor Corporation (an Infineon company) or an affiliate of Cypress Semiconductor Corporation.
