# MTK3339 - Serial

This is a C++ library meant for serial communication with the GPS sensor MTK3339, like the one found in the popular [Adafruit Ultimate GPS v3 module](https://www.adafruit.com/product/746). Suitable for use with Raspberry Pi and similar projects.

## Config

The library contains YAML parsing functionality to configure the sensor. Options include:
- Serial port device file (e.g. "/dev/ttyS0")
- Serial port baud rate (e.g. 57600)
- Sensor update period (e.g. 200ms)
- Which GPS messages (e.g. [GPRMC](https://docs.novatel.com/OEM7/Content/Logs/GPRMC.htm)) will be generated every period
- SBAS (Satellite-based Augmentation System) options

## Dependencies

- For parsing YAML files package uses [yaml-cpp](https://github.com/jbeder/yaml-cpp). It can be installed either following the steps on the repo link, or by running:
```bash
sudo apt-get install libyaml-cpp-dev
```

- Last dependency is [libnmea](https://github.com/jacketizer/libnmea). Installation instruction can be found on the repo link.

## Examples

Example files and usage can be found under **examples** folder. Just run `make` command inside it and executables will be generated.
