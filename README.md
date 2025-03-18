# UNIT QWIIC RPI Module

## Description

The UNIT QWIIC RPI Module is a Qwiic interface designed for the Raspberry Pi (RPi) single-board computer. It enables seamless integration with any Qwiic sensors or devices produced by SparkFun or Unit Electronics. By connecting a Qwiic cable between the Qwiic RPi module and your desired sensor, you can easily stack multiple sensors on the same I2C bus, utilizing only one I2C port on the RPi. This feature is particularly beneficial for compact setups like the Raspberry Pi Zero.

<p align="center">
    <img src="./hardware/resources/UE0052-Pinout-QWIIC-RPI.jpg" alt="Qwiic RPi" width="500"/>
</p>

## Features

- **Plug-and-Play Design**: Simplifies the connection of Qwiic sensors and devices to the Raspberry Pi.
- **I2C Bus Sharing**: Allows multiple sensors to share a single I2C bus, reducing port usage.
- **Compact and Versatile**: Ideal for small form-factor Raspberry Pi models like the RPi Zero.
- **Wide Compatibility**: Works with a variety of Qwiic-enabled sensors and devices.

## Applications

- Rapid prototyping with Qwiic sensors.
- IoT projects requiring multiple sensor inputs.
- Educational projects for learning I2C communication.
- Compact setups with limited GPIO availability.

## Getting Started

### Prerequisites

- A Raspberry Pi (any model with I2C support).
- A Qwiic-enabled sensor or device.
- A Qwiic cable.

### Installation

1. Connect the UNIT QWIIC RPI Module to your Raspberry Pi's GPIO header.
2. Use a Qwiic cable to connect the module to your desired sensor or device.
3. Enable I2C on your Raspberry Pi by running `sudo raspi-config` and navigating to `Interfacing Options > I2C`.
<!-- 
### Example Code

Below is a Python example using the `smbus` library to read data from a Qwiic sensor:

```python
import smbus
import time

# Initialize I2C bus
bus = smbus.SMBus(1)
sensor_address = 0x48  # Replace with your sensor's I2C address

try:
    while True:
        data = bus.read_byte(sensor_address)
        print(f"Sensor Data: {data}")
        time.sleep(1)
except KeyboardInterrupt:
    print("Exiting...")
``` -->

## Resources

- [Qwiic Ecosystem Overview](https://www.sparkfun.com/qwiic)
- [Raspberry Pi Documentation](https://www.raspberrypi.org/documentation/)
- [Python smbus Library](https://pypi.org/project/smbus/)

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.


