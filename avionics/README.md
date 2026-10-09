# Avionics

Flight computer and power system firmware, hardware design files, and supporting tests.

## Flight computer

This is the STM32 flight computer project for the NUCLEO-H5E5ZJ. Open `flight-computer` in STM32CubeIDE as `neptune_avionics_bench`.

Start with the [setup guide](../StartHere.md) and [sensor driver list](docs/sensor-drivers.md). Our first device is the LSM6DSV320X IMU, using the proposed SPI4 connection. Its STM32 functions need timeouts and error reporting.

Inside `flight-computer`, keep generated code in `Core`, ST support in `Drivers` and imported drivers in `ThirdParty`. Our own code can go in `Core/Inc/neptune` and `Core/Src/neptune`. Avionics architecture and connection notes go in `docs`. Sensor communication still needs hardware testing.

